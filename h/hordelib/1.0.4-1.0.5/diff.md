# Comparing `tmp/hordelib-1.0.4.tar.gz` & `tmp/hordelib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-1.0.4.tar", last modified: Thu May 18 15:56:37 2023, max compression
+gzip compressed data, was "hordelib-1.0.5.tar", last modified: Fri May 19 13:29:58 2023, max compression
```

## Comparing `hordelib-1.0.4.tar` & `hordelib-1.0.5.tar`

### file list

```diff
@@ -1,921 +1,920 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.471994 hordelib-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-18 15:56:19.000000 hordelib-1.0.4/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-18 15:56:19.000000 hordelib-1.0.4/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.347993 hordelib-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.363993 hordelib-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-18 15:56:19.000000 hordelib-1.0.4/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-18 15:56:19.000000 hordelib-1.0.4/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-18 15:56:19.000000 hordelib-1.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-18 15:56:19.000000 hordelib-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    41265 2023-05-18 15:56:27.000000 hordelib-1.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-18 15:56:19.000000 hordelib-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-18 15:56:19.000000 hordelib-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-18 15:56:37.471994 hordelib-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-18 15:56:19.000000 hordelib-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-18 15:56:19.000000 hordelib-1.0.4/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.367993 hordelib-1.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/kudos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/make_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/make_index_all_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_all_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_all_stress_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_kudos_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_long_prompt_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_cnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_cnet_preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_stress_test_txt2img_hiresfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_txt2img_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 15:56:19.000000 hordelib-1.0.4/examples/run_upscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.367993 hordelib-1.0.4/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.371993 hordelib-1.0.4/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.371993 hordelib-1.0.4/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.371993 hordelib-1.0.4/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.371993 hordelib-1.0.4/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38661 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/gligen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89264 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.375993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37803 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.379993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.379993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.379993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.379993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.379993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.379993 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    29815 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    46240 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.383993 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.383993 hordelib-1.0.4/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.383993 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.383993 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.387993 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_rebatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/extra_model_paths.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.351993 hordelib-1.0.4/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/gligen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/gligen/put_gligen_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/hypernetworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/hypernetworks/put_hypernetworks_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.391993 hordelib-1.0.4/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    51038 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.395993 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/clipspace.js
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/editAttention.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/keybinds.js
--rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/maskeditor.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/noteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   486763 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    36531 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/_comfyui/web/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/types/comfy.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-05-18 15:56:29.000000 hordelib-1.0.4/hordelib/_comfyui/web/types/litegraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-18 15:56:37.000000 hordelib-1.0.4/hordelib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/blip/caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.399993 hordelib-1.0.4/hordelib/clip/ranking_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/artists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/flavors.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/mediums.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/ranking_lists/techniques.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19874 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    36878 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.403993 hordelib-1.0.4/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_database/med_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.403993 hordelib-1.0.4/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36764 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/model_manager/safety_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.403993 hordelib-1.0.4/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.403993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.403993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.403993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.407993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.355993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.411993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.415994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.419993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.419993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.355993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.419993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.419993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.419993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.419993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.423994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.423994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.423994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.427994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.427994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.427994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.427994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.435994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.435994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.435994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.439994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.439994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.439994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.443994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.443994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.443994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.443994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.359993 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.443994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.443994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.447994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.451994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.455994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.459994 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.463994 hordelib-1.0.4/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.463994 hordelib-1.0.4/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_controlnet_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/preload.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.463994 hordelib-1.0.4/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.463994 hordelib-1.0.4/hordelib/utils/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/dynamicprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/gpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-18 15:56:19.000000 hordelib-1.0.4/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.367993 hordelib-1.0.4/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-18 15:56:37.000000 hordelib-1.0.4/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    50446 2023-05-18 15:56:37.000000 hordelib-1.0.4/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:56:37.000000 hordelib-1.0.4/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 15:56:37.000000 hordelib-1.0.4/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 15:56:37.000000 hordelib-1.0.4/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.467994 hordelib-1.0.4/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-05-18 15:56:19.000000 hordelib-1.0.4/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-18 15:56:29.000000 hordelib-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 15:56:19.000000 hordelib-1.0.4/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-18 15:56:29.000000 hordelib-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:56:37.471994 hordelib-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.471994 hordelib-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.471994 hordelib-1.0.4/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/meta/test_build_helper_import_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:56:37.471994 hordelib-1.0.4/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/model_managers/test_annotators.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/model_managers/test_hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_dynamic_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_horde_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_image_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-18 15:56:19.000000 hordelib-1.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-18 15:56:19.000000 hordelib-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.520708 hordelib-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 13:29:38.000000 hordelib-1.0.5/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-19 13:29:38.000000 hordelib-1.0.5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.408709 hordelib-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.420709 hordelib-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-19 13:29:38.000000 hordelib-1.0.5/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-19 13:29:38.000000 hordelib-1.0.5/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-19 13:29:38.000000 hordelib-1.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-19 13:29:38.000000 hordelib-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    41838 2023-05-19 13:29:48.000000 hordelib-1.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-19 13:29:38.000000 hordelib-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-19 13:29:38.000000 hordelib-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-19 13:29:58.520708 hordelib-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-19 13:29:38.000000 hordelib-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-19 13:29:38.000000 hordelib-1.0.5/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.424708 hordelib-1.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/kudos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/make_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/make_index_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_all_stress_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_kudos_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_long_prompt_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_cnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_cnet_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_stress_test_txt2img_hiresfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_txt2img_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 13:29:38.000000 hordelib-1.0.5/examples/run_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.424708 hordelib-1.0.5/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.428709 hordelib-1.0.5/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38661 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/gligen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27584 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89264 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.432709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37803 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29815 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46240 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.436709 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.440708 hordelib-1.0.5/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.440708 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.440708 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.444708 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.444708 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.444708 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.444708 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_rebatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.444708 hordelib-1.0.5/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/extra_model_paths.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.444708 hordelib-1.0.5/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.412709 hordelib-1.0.5/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/gligen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/gligen/put_gligen_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/hypernetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/hypernetworks/put_hypernetworks_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    51038 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.448708 hordelib-1.0.5/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.452709 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/clipspace.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/editAttention.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/keybinds.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/maskeditor.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/noteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.452709 hordelib-1.0.5/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   486763 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.452709 hordelib-1.0.5/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36531 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.452709 hordelib-1.0.5/hordelib/_comfyui/web/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/types/comfy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-05-19 13:29:50.000000 hordelib-1.0.5/hordelib/_comfyui/web/types/litegraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-19 13:29:58.000000 hordelib-1.0.5/hordelib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.452709 hordelib-1.0.5/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.452709 hordelib-1.0.5/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.456709 hordelib-1.0.5/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.456709 hordelib-1.0.5/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19874 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36878 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.456709 hordelib-1.0.5/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_database/med_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.456709 hordelib-1.0.5/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36751 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/model_manager/safety_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.456709 hordelib-1.0.5/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.460708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.416709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.464708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.468708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.472708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.472708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.416709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.472708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.472708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.472708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.472708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.476709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.476709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.476709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.476709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.476709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.480708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.480708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.484708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.484708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.488708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.488708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.488708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.416709 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.492708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.496708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.500708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.500708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.504708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.508708 hordelib-1.0.5/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.512708 hordelib-1.0.5/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_controlnet_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/preload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.512708 hordelib-1.0.5/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.512708 hordelib-1.0.5/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/dynamicprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/gpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 13:29:38.000000 hordelib-1.0.5/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.428709 hordelib-1.0.5/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50821 2023-05-19 13:29:58.000000 hordelib-1.0.5/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50407 2023-05-19 13:29:58.000000 hordelib-1.0.5/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:29:58.000000 hordelib-1.0.5/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-19 13:29:58.000000 hordelib-1.0.5/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 13:29:58.000000 hordelib-1.0.5/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.516708 hordelib-1.0.5/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-05-19 13:29:38.000000 hordelib-1.0.5/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-19 13:29:50.000000 hordelib-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 13:29:38.000000 hordelib-1.0.5/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-19 13:29:50.000000 hordelib-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:29:58.520708 hordelib-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.520708 hordelib-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.520708 hordelib-1.0.5/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/meta/test_build_helper_import_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:29:58.520708 hordelib-1.0.5/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/model_managers/test_annotators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/model_managers/test_hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_dynamic_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_horde_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-19 13:29:38.000000 hordelib-1.0.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-19 13:29:38.000000 hordelib-1.0.5/tox.ini
```

### Comparing `hordelib-1.0.4/.changelog` & `hordelib-1.0.5/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/.github/workflows/maintests.yml` & `hordelib-1.0.5/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/.github/workflows/prtests.yml` & `hordelib-1.0.5/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/.github/workflows/release.yml` & `hordelib-1.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/.gitignore` & `hordelib-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/CHANGELOG.md` & `hordelib-1.0.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 ## hordelib Changelog
 
+## [v1.0.5](https://github.com/Haidra-Org/hordelib/compare/v1.0.4...v1.0.5)
+
+19 May 2023
+
+- refactor: get_mm_pointers accommodates `type` as well [`1007d69`](https://github.com/Haidra-Org/hordelib/commit/1007d69c5f70bebc2f47f1b1fb41bb24e3282fc5)  (tazlin)
+- fix: unsupport 'diffusers' [`0c9592d`](https://github.com/Haidra-Org/hordelib/commit/0c9592d6579fe3fb1463ed0e2bbba79736d09462)  (tazlin)
+- feat: move stable_diffusion_inpainting if in diffusers directory [`d8ddb01`](https://github.com/Haidra-Org/hordelib/commit/d8ddb01b2ac4f3038098b0e08924aaee0c0b055b)  (tazlin)
+
 ## [v1.0.4](https://github.com/Haidra-Org/hordelib/compare/v1.0.3...v1.0.4)
 
 18 May 2023
 
 - Increase read/write sizes during download/checksums [`#274`](https://github.com/Haidra-Org/hordelib/pull/274) (Andy Pilate)
 - feat: support prepending proxy URL to github downloads [`653a729`](https://github.com/Haidra-Org/hordelib/commit/653a7296a1da400f04d4262e982537de678d2f12)  (tazlin)
 - ci: fix: allow release workflow repo write permissions [`2a8e8d7`](https://github.com/Haidra-Org/hordelib/commit/2a8e8d7356a9310bdb527577a17df386183a8a3e)  (tazlin)
```

### Comparing `hordelib-1.0.4/LICENSE` & `hordelib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/PKG-INFO` & `hordelib-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 1.0.4
+Version: 1.0.5
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-1.0.4/README.md` & `hordelib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/build_helper.py` & `hordelib-1.0.5/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/kudos.py` & `hordelib-1.0.5/examples/kudos.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/make_index.py` & `hordelib-1.0.5/examples/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/make_index_all_models.py` & `hordelib-1.0.5/examples/make_index_all_models.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_all_models.py` & `hordelib-1.0.5/examples/run_all_models.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_all_stress_tests.py` & `hordelib-1.0.5/examples/run_all_stress_tests.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_clip.py` & `hordelib-1.0.5/examples/run_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_controlnet.py` & `hordelib-1.0.5/examples/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_controlnet_annotator.py` & `hordelib-1.0.5/examples/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_facefix.py` & `hordelib-1.0.5/examples/run_facefix.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
 
 def main():
-
     hordelib.initialise()
 
     from PIL import Image
 
     from hordelib.horde import HordeLib
     from hordelib.shared_model_manager import SharedModelManager
 
@@ -19,15 +18,14 @@
     modeltypes = {
         # aitemplate
         "blip": True,
         "clip": True,
         "codeformer": True,
         "compvis": True,
         "controlnet": True,
-        "diffusers": True,
         "esrgan": True,
         "gfpgan": True,
         "safety_checker": True,
     }
 
     SharedModelManager.loadModelManagers(**modeltypes)
     SharedModelManager.manager.load("CodeFormers")
```

### Comparing `hordelib-1.0.4/examples/run_img2img.py` & `hordelib-1.0.5/examples/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_img2img_hires.py` & `hordelib-1.0.5/examples/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_img2img_inpaint.py` & `hordelib-1.0.5/examples/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_img2img_inpaint_mask.py` & `hordelib-1.0.5/examples/run_img2img_inpaint_mask.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     from PIL import Image
 
     from hordelib.horde import HordeLib
     from hordelib.shared_model_manager import SharedModelManager
 
     generate = HordeLib()
-    SharedModelManager.loadModelManagers(compvis=True, diffusers=True)
+    SharedModelManager.loadModelManagers(compvis=True)
     SharedModelManager.manager.load("stable_diffusion_inpainting")
 
     data = {
         "sampler_name": "euler",
         "cfg_scale": 8,
         "denoising_strength": 1,
         "seed": 8369138046008,
```

### Comparing `hordelib-1.0.4/examples/run_img2img_outpaint.py` & `hordelib-1.0.5/examples/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_inpainting.py` & `hordelib-1.0.5/examples/run_inpainting.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
 
 def main():
-
     hordelib.initialise()
 
     from PIL import Image
 
     from hordelib.horde import HordeLib
     from hordelib.shared_model_manager import SharedModelManager
 
     generate = HordeLib()
-    SharedModelManager.loadModelManagers(diffusers=True)
+    SharedModelManager.loadModelManagers(compvis=True)
     SharedModelManager.manager.load("stable_diffusion_inpainting")
 
     data = {
         "sampler_name": "euler",
         "cfg_scale": 8,
         "denoising_strength": 0.72,
         "seed": 836913938046008,
```

### Comparing `hordelib-1.0.4/examples/run_kudos_test.py` & `hordelib-1.0.5/examples/run_kudos_test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_long_prompt_check.py` & `hordelib-1.0.5/examples/run_long_prompt_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,29 @@
         "control_type": None,
         "image_is_control": False,
         "return_control_map": False,
         "prompt": (
             "a dog in a field with a burning bird flying over a blue river with green fish swimming under the surface "
             "all part of an oil painting in the style of Picasso hanging on the wall in an abandoned museum "
             "with old wooden floor boards and a broken window in the background. Outside the window the sun "
-            "is setting and off in the distance can be seen a dog in a field with a burning bird flying over a blue river"
+            "is setting and off in the distance can be seen a dog in a field with a burning bird flying over "
+            "a blue river"
         ),
         "ddim_steps": 50,
         "n_iter": 1,
         "model": "Deliberate",
     }
 
     # Warmup
     generate.basic_inference(basic_data)
 
     i = 1
 
     # Do this a few times to be sure
     for _ in range(3):
-
         # let us enable comfyui's default behaviour of batch optimisations
         UserSettings.enable_batch_optimisations.activate()
         start_clock(f"{i}a. Inference with default comfyui")
         generate.basic_inference(basic_data)
         stop_clock()
 
         # no batch optimisations
@@ -100,15 +100,14 @@
         generate.basic_inference(basic_data)
         stop_clock()
 
         i += 1
 
     # Try the same thing with a really long prompt
     for _ in range(3):
-
         # let us enable comfyui's default behaviour of batch optimisations
         UserSettings.enable_batch_optimisations.activate()
         start_clock(f"{i}a. Long Prompt Inference with default comfyui")
         generate.basic_inference(long_prompt_data)
         stop_clock()
 
         # no batch optimisations
```

### Comparing `hordelib-1.0.4/examples/run_memory_test.py` & `hordelib-1.0.5/examples/run_memory_test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_cnet.py` & `hordelib-1.0.5/examples/run_stress_test_cnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_cnet_preproc.py` & `hordelib-1.0.5/examples/run_stress_test_cnet_preproc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_dynamic.py` & `hordelib-1.0.5/examples/run_stress_test_dynamic.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_img2img.py` & `hordelib-1.0.5/examples/run_stress_test_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_mixed.py` & `hordelib-1.0.5/examples/run_stress_test_mixed.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_pp.py` & `hordelib-1.0.5/examples/run_stress_test_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_txt2img.py` & `hordelib-1.0.5/examples/run_stress_test_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_stress_test_txt2img_hiresfix.py` & `hordelib-1.0.5/examples/run_stress_test_txt2img_hiresfix.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_txt2img.py` & `hordelib-1.0.5/examples/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_txt2img_hires.py` & `hordelib-1.0.5/examples/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_txt2img_local_model.py` & `hordelib-1.0.5/examples/run_txt2img_local_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/examples/run_upscale.py` & `hordelib-1.0.5/examples/run_upscale.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     modeltypes = {
         # aitemplate
         "blip": True,
         "clip": True,
         "codeformer": True,
         "compvis": True,
         "controlnet": True,
-        "diffusers": True,
+        # "diffusers": True,
         "esrgan": True,
         "gfpgan": True,
         "safety_checker": True,
     }
 
     SharedModelManager.loadModelManagers(**modeltypes)
     SharedModelManager.manager.load("RealESRGAN_x4plus")
```

### Comparing `hordelib-1.0.4/hordelib/_comfyui/LICENSE` & `hordelib-1.0.5/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/README.md` & `hordelib-1.0.5/hordelib/_comfyui/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/gligen.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/gligen.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/model_management.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/model_management.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sample.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/samplers.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/samplers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_clip.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-1.0.5/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy/utils.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_hypernetwork.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_mask.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_rebatch.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_rebatch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-1.0.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-1.0.5/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-1.0.5/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/execution.py` & `hordelib-1.0.5/hordelib/_comfyui/execution.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-1.0.5/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/folder_paths.py` & `hordelib-1.0.5/hordelib/_comfyui/folder_paths.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/input/example.png` & `hordelib-1.0.5/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/main.py` & `hordelib-1.0.5/hordelib/_comfyui/main.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-1.0.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/nodes.py` & `hordelib-1.0.5/hordelib/_comfyui/nodes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-1.0.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-1.0.5/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/server.py` & `hordelib-1.0.5/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/clipspace.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/clipspace.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/editAttention.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/editAttention.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/keybinds.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/keybinds.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/maskeditor.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/maskeditor.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/noteNode.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/noteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/slotDefaults.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/slotDefaults.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-1.0.5/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/index.html` & `hordelib-1.0.5/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-1.0.5/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-1.0.5/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/scripts/api.js` & `hordelib-1.0.5/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/scripts/app.js` & `hordelib-1.0.5/hordelib/_comfyui/web/scripts/app.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-1.0.5/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-1.0.5/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-1.0.5/hordelib/_comfyui/web/scripts/ui.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-1.0.5/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/style.css` & `hordelib-1.0.5/hordelib/_comfyui/web/style.css`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/types/comfy.d.ts` & `hordelib-1.0.5/hordelib/_comfyui/web/types/comfy.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/_comfyui/web/types/litegraph.d.ts` & `hordelib-1.0.5/hordelib/_comfyui/web/types/litegraph.d.ts`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/benchmark.py` & `hordelib-1.0.5/hordelib/benchmark.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/blip/caption.py` & `hordelib-1.0.5/hordelib/blip/caption.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/cache/cache.py` & `hordelib-1.0.5/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/bulk.py` & `hordelib-1.0.5/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/coca.py` & `hordelib-1.0.5/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/image.py` & `hordelib-1.0.5/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/interrogate.py` & `hordelib-1.0.5/hordelib/clip/interrogate.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/ranking_lists/artists.txt` & `hordelib-1.0.5/hordelib/clip/ranking_lists/artists.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/ranking_lists/flavors.txt` & `hordelib-1.0.5/hordelib/clip/ranking_lists/flavors.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/ranking_lists/mediums.txt` & `hordelib-1.0.5/hordelib/clip/ranking_lists/mediums.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/ranking_lists/movements.txt` & `hordelib-1.0.5/hordelib/clip/ranking_lists/movements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/ranking_lists/tags.txt` & `hordelib-1.0.5/hordelib/clip/ranking_lists/tags.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/ranking_lists/techniques.txt` & `hordelib-1.0.5/hordelib/clip/ranking_lists/techniques.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/clip/text.py` & `hordelib-1.0.5/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/comfy_horde.py` & `hordelib-1.0.5/hordelib/comfy_horde.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/config_path.py` & `hordelib-1.0.5/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/consts.py` & `hordelib-1.0.5/hordelib/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,52 +29,52 @@
     """Look up str enum for the categories of models (compvis, controlnet, clip, etc...)."""
 
     blip = "blip"
     clip = "clip"
     codeformer = "codeformer"
     compvis = "compvis"
     controlnet = "controlnet"
-    diffusers = "diffusers"
+    # diffusers = "diffusers"
     esrgan = "esrgan"
     gfpgan = "gfpgan"
     safety_checker = "safety_checker"
 
 
 # Default model managers to load
 DEFAULT_MODEL_MANAGERS = {
     MODEL_CATEGORY_NAMES.blip: True,
     MODEL_CATEGORY_NAMES.clip: True,
     MODEL_CATEGORY_NAMES.codeformer: True,
     MODEL_CATEGORY_NAMES.compvis: True,
     MODEL_CATEGORY_NAMES.controlnet: True,
-    MODEL_CATEGORY_NAMES.diffusers: True,
+    # MODEL_CATEGORY_NAMES.diffusers: True,
     MODEL_CATEGORY_NAMES.esrgan: True,
     MODEL_CATEGORY_NAMES.gfpgan: True,
     MODEL_CATEGORY_NAMES.safety_checker: True,
 }
 """The default model managers to load."""  # XXX Clarify
 
 MODEL_DB_NAMES = {
     MODEL_CATEGORY_NAMES.blip: MODEL_CATEGORY_NAMES.blip,
     MODEL_CATEGORY_NAMES.clip: MODEL_CATEGORY_NAMES.clip,
     MODEL_CATEGORY_NAMES.codeformer: MODEL_CATEGORY_NAMES.codeformer,
     MODEL_CATEGORY_NAMES.compvis: "stable_diffusion",
     MODEL_CATEGORY_NAMES.controlnet: MODEL_CATEGORY_NAMES.controlnet,
-    MODEL_CATEGORY_NAMES.diffusers: MODEL_CATEGORY_NAMES.diffusers,
+    # MODEL_CATEGORY_NAMES.diffusers: MODEL_CATEGORY_NAMES.diffusers,
     MODEL_CATEGORY_NAMES.esrgan: MODEL_CATEGORY_NAMES.esrgan,
     MODEL_CATEGORY_NAMES.gfpgan: MODEL_CATEGORY_NAMES.gfpgan,
     MODEL_CATEGORY_NAMES.safety_checker: MODEL_CATEGORY_NAMES.safety_checker,
 }
 """The name of the json file (without the extension) of the corresponding model database."""
 
 MODEL_FOLDER_NAMES = {
     MODEL_CATEGORY_NAMES.blip: MODEL_CATEGORY_NAMES.blip,
     MODEL_CATEGORY_NAMES.clip: MODEL_CATEGORY_NAMES.clip,
     MODEL_CATEGORY_NAMES.codeformer: MODEL_CATEGORY_NAMES.codeformer,
     MODEL_CATEGORY_NAMES.compvis: "compvis",
     MODEL_CATEGORY_NAMES.controlnet: MODEL_CATEGORY_NAMES.controlnet,
-    MODEL_CATEGORY_NAMES.diffusers: MODEL_CATEGORY_NAMES.diffusers,
+    # MODEL_CATEGORY_NAMES.diffusers: MODEL_CATEGORY_NAMES.diffusers,
     MODEL_CATEGORY_NAMES.esrgan: MODEL_CATEGORY_NAMES.esrgan,
     MODEL_CATEGORY_NAMES.gfpgan: MODEL_CATEGORY_NAMES.gfpgan,
     MODEL_CATEGORY_NAMES.safety_checker: MODEL_CATEGORY_NAMES.safety_checker,
 }
 """The folder name on disk where the models are stored in AIWORKER_CACHE_HOME."""
```

### Comparing `hordelib-1.0.4/hordelib/horde.py` & `hordelib-1.0.5/hordelib/horde.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/initialisation.py` & `hordelib-1.0.5/hordelib/initialisation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/install_comfy.patch` & `hordelib-1.0.5/hordelib/install_comfy.patch`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/install_comfy.py` & `hordelib-1.0.5/hordelib/install_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_database/db_dep.json` & `hordelib-1.0.5/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_database/db_embeds.json` & `hordelib-1.0.5/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_database/diffusers.json` & `hordelib-1.0.5/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/base.py` & `hordelib-1.0.5/hordelib/model_manager/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         """
         Returns the available models
         """
         return self.available_models
 
     def get_available_models_by_types(self, model_types: list[str] | None = None):
         if not model_types:
-            model_types = ["ckpt", "diffusers"]
+            model_types = ["ckpt"]
         models_available = []
         for model in self.model_reference:
             if self.model_reference[model]["type"] in model_types and self.check_available(
                 self.get_model_files(model),
             ):
                 models_available.append(model)
         return models_available
```

### Comparing `hordelib-1.0.4/hordelib/model_manager/blip.py` & `hordelib-1.0.5/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/clip.py` & `hordelib-1.0.5/hordelib/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/codeformer.py` & `hordelib-1.0.5/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/compvis.py` & `hordelib-1.0.5/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/controlnet.py` & `hordelib-1.0.5/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/esrgan.py` & `hordelib-1.0.5/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/gfpgan.py` & `hordelib-1.0.5/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/model_manager/hyper.py` & `hordelib-1.0.5/hordelib/model_manager/hyper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 import torch
 from loguru import logger
 
 from hordelib.consts import EXCLUDED_MODEL_NAMES, MODEL_CATEGORY_NAMES
 
 # from hordelib.model_manager.aitemplate import AITemplateModelManager
+# from hordelib.model_manager.diffusers import DiffusersModelManager
 from hordelib.model_manager.base import BaseModelManager
 from hordelib.model_manager.blip import BlipModelManager
 from hordelib.model_manager.clip import ClipModelManager
 from hordelib.model_manager.codeformer import CodeFormerModelManager
 from hordelib.model_manager.compvis import CompVisModelManager
 from hordelib.model_manager.controlnet import ControlNetModelManager
-from hordelib.model_manager.diffusers import DiffusersModelManager
 from hordelib.model_manager.esrgan import EsrganModelManager
 from hordelib.model_manager.gfpgan import GfpganModelManager
 from hordelib.model_manager.safety_checker import SafetyCheckerModelManager
 
 MODEL_MANAGERS_TYPE_LOOKUP: dict[MODEL_CATEGORY_NAMES, type[BaseModelManager]] = {
     # ModelCategoryNames.aitemplate: AITemplateModelManager,
     MODEL_CATEGORY_NAMES.blip: BlipModelManager,
     MODEL_CATEGORY_NAMES.clip: ClipModelManager,
     MODEL_CATEGORY_NAMES.codeformer: CodeFormerModelManager,
     MODEL_CATEGORY_NAMES.compvis: CompVisModelManager,
     MODEL_CATEGORY_NAMES.controlnet: ControlNetModelManager,
-    MODEL_CATEGORY_NAMES.diffusers: DiffusersModelManager,
+    # MODEL_CATEGORY_NAMES.diffusers: DiffusersModelManager,
     MODEL_CATEGORY_NAMES.esrgan: EsrganModelManager,
     MODEL_CATEGORY_NAMES.gfpgan: GfpganModelManager,
     MODEL_CATEGORY_NAMES.safety_checker: SafetyCheckerModelManager,
 }
 """Keys are `str` which represent attrs in `ModelManger`. Values are the corresponding `type`."""
 
 
@@ -39,45 +39,53 @@
 
     # aitemplate: AITemplateModelManager | None = None
     blip: BlipModelManager | None = None
     clip: ClipModelManager | None = None
     codeformer: CodeFormerModelManager | None = None
     compvis: CompVisModelManager | None = None
     controlnet: ControlNetModelManager | None = None
-    diffusers: DiffusersModelManager | None = None
+    # diffusers: DiffusersModelManager | None = None
     esrgan: EsrganModelManager | None = None
     gfpgan: GfpganModelManager | None = None
     safety_checker: SafetyCheckerModelManager | None = None
     # XXX I think this can be reworked into an array of BaseModelManager instances
 
     @property
     def models(self) -> dict:
         """All model manager's internal dictionaries of models, loaded from model database JSON files."""
         _models: dict = {}
         for model_manager in self.active_model_managers:
             model_manager.model_reference
             _models.update(model_manager.model_reference)
         return _models
 
-    def get_available_models(self, mm_include=None, mm_exclude=None) -> list[str]:
+    def get_available_models(
+        self,
+        mm_include: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] = None,
+        mm_exclude: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] = None,
+    ) -> list[str]:
         """All models for which information exists, and for which a download attempt could be made."""
         all_available_models: list[str] = []
         mm_include = self.get_mm_pointers(mm_include)
         mm_exclude = self.get_mm_pointers(mm_exclude)
         for model_manager in self.active_model_managers:
             if mm_include and model_manager not in mm_include:
                 continue
             if mm_exclude and model_manager in mm_exclude:
                 continue
             all_available_models.extend(model_manager.available_models)
         return all_available_models
 
     available_models = property(get_available_models)
 
-    def get_loaded_models(self, mm_include=None, mm_exclude=None) -> dict[str, dict]:
+    def get_loaded_models(
+        self,
+        mm_include: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] = None,
+        mm_exclude: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] = None,
+    ) -> dict[str, dict]:
         """All models for which have successfully loaded across all `BaseModelManager` types."""
         all_loaded_models: dict[str, dict] = {}
         mm_include = self.get_mm_pointers(mm_include)
         mm_exclude = self.get_mm_pointers(mm_exclude)
         for model_manager in self.active_model_managers:
             if mm_include and model_manager not in mm_include:
                 continue
@@ -92,15 +100,15 @@
     def active_model_managers(self) -> list[BaseModelManager]:
         """All loaded model managers."""
         all_model_managers = [
             # self.aitemplate, # XXX TODO
             self.blip,
             self.clip,
             self.compvis,
-            self.diffusers,
+            # self.diffusers,
             self.esrgan,
             self.gfpgan,
             self.safety_checker,
             self.codeformer,
             self.controlnet,
         ]
         # reset available models
@@ -133,15 +141,15 @@
         self,
         # aitemplate: bool = False, # XXX
         blip: bool = False,
         clip: bool = False,
         codeformer: bool = False,
         compvis: bool = False,
         controlnet: bool = False,
-        diffusers: bool = False,
+        # diffusers: bool = False,
         esrgan: bool = False,
         gfpgan: bool = False,
         safety_checker: bool = False,
     ):  # XXX are we married to the name and/or the idea behind this function
         """For each arg which is true, attempt to load that `BaseModelManager` type."""
         args_passed: dict = locals().copy()  # XXX This is temporary
         args_passed.pop("self")  # XXX This is temporary
@@ -224,17 +232,14 @@
         Returns:
             bool | None: The result of the validation. If `None`, the model was not found.
         """
         for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_manager: BaseModelManager = getattr(self, model_manager_type)
             if model_manager is None:
                 continue
-            if model_manager_type == "aitemplate":
-                continue
-                # XXX the special handling here predates me (@tazlin), unknown if needed
             if model_name in model_manager.model_reference:
                 return model_manager.validate_model(model_name, skip_checksum)
         return None
 
     def taint_models(self, models: list[str]) -> None:
         """Marks a list of models to be unavailable.
 
@@ -280,30 +285,32 @@
                 continue
             if model_name in model_manager.model_reference or model_manager.is_local_model(model_name):
                 return model_manager.move_from_disk_cache(model_name, model, clip, vae)
         return None
 
     def get_loaded_models_names(
         self,
-        mm_include: list[str] | None = None,
-        mm_exclude: list[str] | None = None,
+        mm_include: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] | None = None,
+        mm_exclude: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] | None = None,
     ) -> list:
         """
         Returns:
             list: All currently loaded models.
         """
         loaded_models = self.get_loaded_models(mm_include, mm_exclude)
         return list(loaded_models.keys())
 
     def is_model_loaded(self, model_name) -> bool:
         return model_name in self.loaded_models
 
-    def get_available_models_by_types(self, mm_include: list[str] | None = None, mm_exclude: list[str] | None = None):
-        if not mm_include and not mm_exclude:
-            mm_include = ["ckpt", "diffusers"]
+    def get_available_models_by_types(
+        self,
+        mm_include: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] | None = None,
+        mm_exclude: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] | None = None,
+    ):
         return self.get_available_models(mm_include, mm_exclude)
 
     def count_available_models_by_types(
         self,
         model_types: list[str] | None = None,
     ) -> int:
         return len(self.get_available_models_by_types(model_types))
@@ -360,30 +367,26 @@
                     gpu_id=gpu_id,
                     cpu_only=cpu_only,
                 )
 
         logger.error(f"{model_name} not found")
         return None
 
-    def get_mm_pointers(self, mm_types: list[str] | None = None):
-        mm_pointers = set()
+    def get_mm_pointers(self, mm_types: list[str | MODEL_CATEGORY_NAMES | type[BaseModelManager]] | None = None):
         if not mm_types:
-            return mm_pointers
-        # If any value in the list is not a string, we assume it's a mm pointer already but we verify
-        if any(type(mm_type) != str for mm_type in mm_types):
-            for mm_type in mm_types:
-                for active_mm in self.active_model_managers:
-                    if active_mm == mm_type:
-                        mm_pointers.add(active_mm)
-                        break
+            return set()
+
+        active_model_managers_types = [type(model_manager) for model_manager in self.active_model_managers]
+
+        resolved_types = []
         for mm_type in mm_types:
-            if type(mm_type) != str:
+            if mm_type in active_model_managers_types:
+                resolved_types.append(mm_type)
                 continue
-            try:
-                mm_type = MODEL_MANAGERS_TYPE_LOOKUP[MODEL_CATEGORY_NAMES(mm_type)]
-            except Exception as err:
-                logger.warning(f"Exception when looking up model manager '{mm_type}': {err}")
-            for active_mm in self.active_model_managers:
-                if type(active_mm) == mm_type:
-                    mm_pointers.add(active_mm)
-                    break
-        return mm_pointers
+
+            if mm_type in MODEL_MANAGERS_TYPE_LOOKUP:
+                if MODEL_MANAGERS_TYPE_LOOKUP[mm_type] not in active_model_managers_types:
+                    logger.warning(f"Attempted to reference a model manager which isn't loaded: '{mm_type}'.")
+                else:
+                    resolved_types.append(MODEL_MANAGERS_TYPE_LOOKUP[mm_type])
+
+        return {mm for mm in self.active_model_managers if type(mm) in resolved_types}
```

### Comparing `hordelib-1.0.4/hordelib/model_manager/safety_checker.py` & `hordelib-1.0.5/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-1.0.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/__init__.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-1.0.5/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/node_clip_similarities.py` & `hordelib-1.0.5/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-1.0.5/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/node_image_loader.py` & `hordelib-1.0.5/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/node_image_output.py` & `hordelib-1.0.5/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/node_model_loader.py` & `hordelib-1.0.5/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-1.0.5/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_controlnet_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-1.0.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_controlnet_hires_fix.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_controlnet_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-1.0.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/preload.py` & `hordelib-1.0.5/hordelib/preload.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/safety_checker.py` & `hordelib-1.0.5/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/settings.py` & `hordelib-1.0.5/hordelib/settings.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/shared_model_manager.py` & `hordelib-1.0.5/hordelib/shared_model_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,47 @@
 from hordelib.preload import (
     ANNOTATOR_MODEL_SHA_LOOKUP,
     download_all_controlnet_annotators,
     validate_all_controlnet_annotators,
 )
 
 
+def do_migrations():
+    """This function should handle any moving of folders or other restructuring from previous versions."""
+
+    diffusers_dir = Path(get_cache_directory()).joinpath("diffusers")
+    sd_inpainting_v1_5_ckpt = diffusers_dir.joinpath("sd-v1-5-inpainting.ckpt").resolve()
+    sd_inpainting_v1_5_sha256 = diffusers_dir.joinpath("sd-v1-5-inpainting.sha256").resolve()
+    if diffusers_dir.exists() and sd_inpainting_v1_5_ckpt.exists():
+        logger.init_warn(
+            "stable_diffusion_inpainting found in diffusers folder and is being moved to compvis",
+            status="Warning",
+        )
+
+        target_ckpt_path = Path(get_cache_directory()).joinpath("compvis").joinpath("sd-v1-5-inpainting.ckpt")
+        target_sha_path = Path(get_cache_directory()).joinpath("compvis").joinpath("sd-v1-5-inpainting.sha256")
+
+        try:
+            sd_inpainting_v1_5_ckpt.rename(target_ckpt_path)
+            if sd_inpainting_v1_5_sha256.exists():
+                sd_inpainting_v1_5_sha256.rename(target_sha_path)
+        except OSError as e:
+            logger.init_err(
+                f"Failed to move {sd_inpainting_v1_5_ckpt} to {target_ckpt_path}. {e}",
+                status="Error",
+            )
+            logger.init_err("Please move this file manually and try again.", status="Error")
+            return
+
+        logger.init_warn(
+            "stable_diffusion_inpainting successfully moved to compvis. The diffusers directory can now be deleted.",
+            status="Warning",
+        )
+
+
 class SharedModelManager:
     _instance = None
     manager: ModelManager | None = None
 
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
@@ -33,15 +66,15 @@
         cls,
         # aitemplate: bool = False,
         blip: bool = False,
         clip: bool = False,
         codeformer: bool = False,
         compvis: bool = False,
         controlnet: bool = False,
-        diffusers: bool = False,
+        # diffusers: bool = False,
         esrgan: bool = False,
         gfpgan: bool = False,
         safety_checker: bool = False,
     ):
         if cls.manager is None:
             cls.manager = ModelManager()
 
@@ -51,15 +84,15 @@
         db_reference_files_lookup = download_live_legacy_dbs(override_existing=True, proxy_url=REMOTE_PROXY)
         for model_db, file_path in db_reference_files_lookup.items():
             hordelib_model_db_path = get_model_reference_filename(
                 model_db,
                 base_path=Path(get_hordelib_path()).joinpath("model_database"),
             )
             try:
-                logger.debug(f"Unlinking {hordelib_model_db_path} if it exists.")
+                logger.debug(f"Downloading {hordelib_model_db_path.name}...")
                 hordelib_model_db_path.unlink(missing_ok=True)
                 with open(hordelib_model_db_path, "wb") as f:
                     f.write(file_path.read_bytes())
             except OSError as e:
                 if hordelib_model_db_path.is_symlink():
                     logger.init_err("Failed to unlink symlink.", status="Error")
                     logger.init_err(f"Please delete the symlink at {hordelib_model_db_path} and try again.")
@@ -69,14 +102,15 @@
                         status="Error",
                     )
                     logger.init_err(
                         f"If you continue to get this error, please delete {hordelib_model_db_path}.",
                         status="Error",
                     )
                 raise e
+        do_migrations()
         cls.manager.init_model_managers(**args_passed)
 
     @staticmethod
     def preloadAnnotators() -> bool:
         """Preload all annotators. If they are already downloaded, this will only ensure the SHA256 integrity.
 
         Returns:
```

### Comparing `hordelib-1.0.4/hordelib/train.py` & `hordelib-1.0.5/hordelib/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/blip/blip.py` & `hordelib-1.0.5/hordelib/utils/blip/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/blip/med.py` & `hordelib-1.0.5/hordelib/utils/blip/med.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/blip/vit.py` & `hordelib-1.0.5/hordelib/utils/blip/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/cast.py` & `hordelib-1.0.5/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/dynamicprompt.py` & `hordelib-1.0.5/hordelib/utils/dynamicprompt.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/gpuinfo.py` & `hordelib-1.0.5/hordelib/utils/gpuinfo.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/ioredirect.py` & `hordelib-1.0.5/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib/utils/logger.py` & `hordelib-1.0.5/hordelib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/hordelib.egg-info/PKG-INFO` & `hordelib-1.0.5/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 1.0.4
+Version: 1.0.5
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-1.0.4/hordelib.egg-info/SOURCES.txt` & `hordelib-1.0.5/hordelib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -763,10 +763,9 @@
 tests/test_initialisation.py
 tests/test_safety_checker.py
 tests/test_shared_model_manager.py
 tests/test_utils.py
 tests/meta/test_build_helper_import_check.py
 tests/model_managers/test_annotators.py
 tests/model_managers/test_comvis.py
-tests/model_managers/test_diffusers.py
 tests/model_managers/test_hyper.py
 tests/model_managers/test_safety_checker.py
```

### Comparing `hordelib-1.0.4/images/test_annotator.jpg` & `hordelib-1.0.5/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_db0.jpg` & `hordelib-1.0.5/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_facefix.png` & `hordelib-1.0.5/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_inpaint.png` & `hordelib-1.0.5/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_inpaint_alpha.png` & `hordelib-1.0.5/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_inpaint_mask.png` & `hordelib-1.0.5/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_inpaint_original.png` & `hordelib-1.0.5/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/images/test_outpaint.png` & `hordelib-1.0.5/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/pyproject.toml` & `hordelib-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/requirements.txt` & `hordelib-1.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/model_managers/test_annotators.py` & `hordelib-1.0.5/tests/model_managers/test_annotators.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/model_managers/test_comvis.py` & `hordelib-1.0.5/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/model_managers/test_hyper.py` & `hordelib-1.0.5/tests/model_managers/test_hyper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # test_horde.py
 import pytest
 from PIL import Image
 
+import hordelib
+
+hordelib.initialise()
+
 from hordelib.horde import HordeLib
+from hordelib.model_manager.compvis import CompVisModelManager
+from hordelib.model_manager.esrgan import EsrganModelManager
 from hordelib.shared_model_manager import SharedModelManager
 
 
 class TestHyperMM:
     @pytest.fixture(autouse=True, scope="class")
     def setup_and_teardown(self):
         TestHyperMM.horde = HordeLib()
@@ -78,9 +84,16 @@
         assert len(SharedModelManager.manager.get_mm_pointers(["compvis", "gfpgan"])) == 1
         assert len(SharedModelManager.manager.get_mm_pointers(["compvis", "gfpgan", "esrgan"])) == 2
         assert len(SharedModelManager.manager.get_mm_pointers(["compvis", "FAKE"])) == 1
         assert SharedModelManager.manager.get_mm_pointers(None) == set()
         # Any value other than a string or a mm pointer is ignored
         assert SharedModelManager.manager.get_mm_pointers([None]) == set()
         assert SharedModelManager.manager.get_mm_pointers(
-            [None, SharedModelManager.manager.compvis, "FAKE", "esrgan", "compvis"],
+            [None, "FAKE", "esrgan", "compvis"],
+        ) == {SharedModelManager.manager.compvis, SharedModelManager.manager.esrgan}
+
+        assert SharedModelManager.manager.get_mm_pointers(
+            [EsrganModelManager, CompVisModelManager],
+        ) == {SharedModelManager.manager.compvis, SharedModelManager.manager.esrgan}
+        assert SharedModelManager.manager.get_mm_pointers(
+            [None, "FAKE", EsrganModelManager, CompVisModelManager],
         ) == {SharedModelManager.manager.compvis, SharedModelManager.manager.esrgan}
```

### Comparing `hordelib-1.0.4/tests/model_managers/test_safety_checker.py` & `hordelib-1.0.5/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_blip.py` & `hordelib-1.0.5/tests/test_blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_clip.py` & `hordelib-1.0.5/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_comfy.py` & `hordelib-1.0.5/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_dynamic_prompt.py` & `hordelib-1.0.5/tests/test_dynamic_prompt.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_horde_controlnet_annotator.py` & `hordelib-1.0.5/tests/test_horde_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_horde_inference.py` & `hordelib-1.0.5/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_horde_inference_controlnet.py` & `hordelib-1.0.5/tests/test_horde_inference_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_horde_inference_img2img.py` & `hordelib-1.0.5/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_horde_inference_painting.py` & `hordelib-1.0.5/tests/test_horde_inference_painting.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,32 @@
         self.horde = HordeLib()
 
         self.default_model_manager_args = {
             # aitemplate
             # "blip": True,
             # "clip": True,
             # "codeformer": True,
-            # "compvis": True,
+            "compvis": True,
             # "controlnet": True,
-            "diffusers": True,
+            # "diffusers": True,
             # "esrgan": True,
             # "gfpgan": True,
             # "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         yield
         del self.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
     def test_inpainting_alpha_mask(self):
         SharedModelManager.manager.load("stable_diffusion_inpainting")
         assert (
-            SharedModelManager.manager.diffusers.is_model_loaded(
+            SharedModelManager.manager.compvis.is_model_loaded(
                 "stable_diffusion_inpainting",
             )
             is True
         )
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
@@ -58,15 +58,15 @@
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
         pil_image.save("images/horde_inpainting_alpha_mask.webp", quality=90)
 
     def test_inpainting_separate_mask(self):
         SharedModelManager.manager.load("stable_diffusion_inpainting")
         assert (
-            SharedModelManager.manager.diffusers.is_model_loaded(
+            SharedModelManager.manager.compvis.is_model_loaded(
                 "stable_diffusion_inpainting",
             )
             is True
         )
         data = {
             "sampler_name": "euler",
             "cfg_scale": 8,
```

### Comparing `hordelib-1.0.4/tests/test_horde_pp.py` & `hordelib-1.0.5/tests/test_horde_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_horde_samplers.py` & `hordelib-1.0.5/tests/test_horde_samplers.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_image_metadata.py` & `hordelib-1.0.5/tests/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_inference.py` & `hordelib-1.0.5/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_safety_checker.py` & `hordelib-1.0.5/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tests/test_shared_model_manager.py` & `hordelib-1.0.5/tests/test_shared_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.default_model_manager_args = {  # XXX # TODO
             # aitemplate
             "blip": True,
             "clip": True,
             "codeformer": True,
             "compvis": True,
             "controlnet": True,
-            "diffusers": True,
+            # "diffusers": True,
             "esrgan": True,
             "gfpgan": True,
             "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         yield
@@ -50,15 +50,15 @@
         assert SharedModelManager.manager is not None
         # assert SharedModelManager.manager.aitemplate is not None # XXX # FIXME
         assert SharedModelManager.manager.blip is not None  # XXX
         assert SharedModelManager.manager.clip is not None
         assert SharedModelManager.manager.codeformer is not None
         assert SharedModelManager.manager.compvis is not None
         assert SharedModelManager.manager.controlnet is not None
-        assert SharedModelManager.manager.diffusers is not None
+        # assert SharedModelManager.manager.diffusers is not None
         assert SharedModelManager.manager.esrgan is not None
         assert SharedModelManager.manager.gfpgan is not None
         assert SharedModelManager.manager.safety_checker is not None
 
     def test_horde_model_manager_reload_db(self):
         assert SharedModelManager.manager is not None
         SharedModelManager.manager.reload_database()
```

### Comparing `hordelib-1.0.4/tests/test_utils.py` & `hordelib-1.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-1.0.4/tox.ini` & `hordelib-1.0.5/tox.ini`

 * *Files identical despite different names*

