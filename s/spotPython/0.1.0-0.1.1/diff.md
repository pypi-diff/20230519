# Comparing `tmp/spotPython-0.1.0.tar.gz` & `tmp/spotPython-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.1.0.tar", last modified: Sun May 14 13:57:24 2023, max compression
+gzip compressed data, was "spotPython-0.1.1.tar", last modified: Thu May 18 16:33:28 2023, max compression
```

## Comparing `spotPython-0.1.0.tar` & `spotPython-0.1.1.tar`

### file list

```diff
@@ -1,162 +1,197 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.647561 spotPython-0.1.0/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.605660 spotPython-0.1.0/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.609198 spotPython-0.1.0/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    10054 2023-05-14 06:59:57.000000 spotPython-0.1.0/.gitignore
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.620375 spotPython-0.1.0/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.1.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.1.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.1.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.1.0/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.1.0/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.1.0/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     3718 2023-05-14 13:57:24.647389 spotPython-0.1.0/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2948 2023-02-01 14:33:52.000000 spotPython-0.1.0/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.621910 spotPython-0.1.0/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       49 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)      559 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/gen_ref_pages.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.622217 spotPython-0.1.0/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      100 2023-02-01 14:33:52.000000 spotPython-0.1.0/docs/index.md
--rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.1.0/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.1.0/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.634820 spotPython-0.1.0/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    28141 2023-05-08 22:27:05.000000 spotPython-0.1.0/notebooks/00_spot_doc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.1.0/notebooks/01_spot_intro.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8779 2023-05-08 22:28:10.000000 spotPython-0.1.0/notebooks/02_spot_multidim.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.1.0/notebooks/03_spot_anisotropic.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.1.0/notebooks/04_spot_sklearn_surrogate.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.1.0/notebooks/05_spot_sklearn_optimizers.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.1.0/notebooks/06_spot_gaussian.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.1.0/notebooks/07_spot_ei.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.1.0/notebooks/08_spot_noisy.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.1.0/notebooks/09_spot_ocba.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   125632 2023-05-09 18:52:37.000000 spotPython-0.1.0/notebooks/10_spot_hpt_sklearn_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   293194 2023-05-13 19:51:30.000000 spotPython-0.1.0/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    53313 2023-04-28 11:46:54.000000 spotPython-0.1.0/notebooks/12_spot_hpt_torch_720.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   163882 2023-05-13 22:09:38.000000 spotPython-0.1.0/notebooks/12_spot_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   289738 2023-05-13 22:39:29.000000 spotPython-0.1.0/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   347673 2023-05-14 13:55:19.000000 spotPython-0.1.0/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)  1150881 2023-05-13 19:25:30.000000 spotPython-0.1.0/notebooks/14_spot_ray_hpt_torch_cifar10_360.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    26701 2023-05-09 18:39:01.000000 spotPython-0.1.0/notebooks/15_spot_hpt_sklearn_regression.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36248 2023-05-10 07:18:33.000000 spotPython-0.1.0/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.606046 spotPython-0.1.0/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.635330 spotPython-0.1.0/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.1.0/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.1.0/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.636767 spotPython-0.1.0/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.1.0/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.1.0/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.1.0/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-05-09 06:26:54.000000 spotPython-0.1.0/notebooks/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-14 10:59:48.000000 spotPython-0.1.0/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-14 13:57:24.647596 spotPython-0.1.0/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.606289 spotPython-0.1.0/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.636998 spotPython-0.1.0/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      216 2023-05-14 13:57:24.000000 spotPython-0.1.0/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.637773 spotPython-0.1.0/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.1.0/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.638022 spotPython-0.1.0/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.1.0/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.1.0/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.639505 spotPython-0.1.0/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.1.0/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.1.0/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)    20734 2023-05-09 23:08:47.000000 spotPython-0.1.0/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.1.0/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     4082 2023-05-12 15:44:39.000000 spotPython-0.1.0/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.1.0/src/spotPython/data/torch_hyper_dict.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.640033 spotPython-0.1.0/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.1.0/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.1.0/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.1.0/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.640560 spotPython-0.1.0/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     4163 2023-05-09 19:03:26.000000 spotPython-0.1.0/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     4758 2023-05-13 19:28:44.000000 spotPython-0.1.0/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.1.0/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.640873 spotPython-0.1.0/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.1.0/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)    26028 2023-05-07 10:48:32.000000 spotPython-0.1.0/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.641171 spotPython-0.1.0/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-02-02 22:52:12.000000 spotPython-0.1.0/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-04-22 20:39:46.000000 spotPython-0.1.0/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.641296 spotPython-0.1.0/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    32443 2023-05-12 15:27:01.000000 spotPython-0.1.0/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.641789 spotPython-0.1.0/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)      851 2023-05-12 15:50:08.000000 spotPython-0.1.0/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      309 2023-05-12 15:41:17.000000 spotPython-0.1.0/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      642 2023-05-12 15:50:08.000000 spotPython-0.1.0/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)    14433 2023-05-14 07:44:14.000000 spotPython-0.1.0/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.643324 spotPython-0.1.0/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.1.0/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.1.0/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.1.0/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     1415 2023-05-09 21:08:31.000000 spotPython-0.1.0/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.1.0/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.1.0/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.1.0/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)      936 2023-05-13 15:24:05.000000 spotPython-0.1.0/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     3402 2023-05-09 19:18:13.000000 spotPython-0.1.0/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.1.0/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.1.0/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.1.0/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.637668 spotPython-0.1.0/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     3718 2023-05-14 13:57:24.000000 spotPython-0.1.0/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     5844 2023-05-14 13:57:24.000000 spotPython-0.1.0/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-14 13:57:24.000000 spotPython-0.1.0/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-14 13:57:24.000000 spotPython-0.1.0/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-14 13:57:24.000000 spotPython-0.1.0/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-14 13:57:24.647152 spotPython-0.1.0/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.1.0/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.1.0/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.1.0/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.1.0/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-02-01 14:33:52.000000 spotPython-0.1.0/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.906689 spotPython-0.1.1/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.849082 spotPython-0.1.1/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.853359 spotPython-0.1.1/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    10089 2023-05-15 06:49:11.000000 spotPython-0.1.1/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 11:16:54.000000 spotPython-0.1.1/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.863391 spotPython-0.1.1/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-05-03 09:52:04.000000 spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-08 06:28:53.000000 spotPython-0.1.1/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.1.1/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-25 06:56:48.000000 spotPython-0.1.1/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     3718 2023-05-18 16:33:28.906504 spotPython-0.1.1/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2948 2023-02-01 14:33:52.000000 spotPython-0.1.1/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.868543 spotPython-0.1.1/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)   129512 2023-05-18 12:00:29.000000 spotPython-0.1.1/docs/bart23e.html
+-rw-r--r--   0 bartz      (501) staff       (20)   480591 2023-05-18 12:00:38.000000 spotPython-0.1.1/docs/bart23e.pdf
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.871691 spotPython-0.1.1/docs/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)   109809 2023-05-18 11:26:21.000000 spotPython-0.1.1/docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_contour_0_2.png
+-rw-r--r--   0 bartz      (501) staff       (20)    87479 2023-05-18 11:26:39.000000 spotPython-0.1.1/docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    98660 2023-05-18 11:24:50.000000 spotPython-0.1.1/docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_contour_2_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    20101 2023-05-18 11:26:56.000000 spotPython-0.1.1/docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    25754 2023-05-18 11:27:13.000000 spotPython-0.1.1/docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    98858 2023-05-18 07:56:22.000000 spotPython-0.1.1/docs/figures/parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-18 12:00:38.000000 spotPython-0.1.1/docs/index.html
+-rw-r--r--   0 bartz      (501) staff       (20)    42271 2023-05-18 12:00:38.000000 spotPython-0.1.1/docs/search.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.849728 spotPython-0.1.1/docs/site_libs/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.875060 spotPython-0.1.1/docs/site_libs/bootstrap/
+-rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.1.1/docs/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-18 12:00:28.000000 spotPython-0.1.1/docs/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.875575 spotPython-0.1.1/docs/site_libs/clipboard/
+-rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.877034 spotPython-0.1.1/docs/site_libs/quarto-html/
+-rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-18 11:18:42.000000 spotPython-0.1.1/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.877262 spotPython-0.1.1/docs/site_libs/quarto-nav/
+-rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.878046 spotPython-0.1.1/docs/site_libs/quarto-search/
+-rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.1.1/docs/site_libs/quarto-search/quarto-search.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.879792 spotPython-0.1.1/docs_old/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       49 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)      559 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/gen_ref_pages.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.880177 spotPython-0.1.1/docs_old/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      100 2023-02-01 14:33:52.000000 spotPython-0.1.1/docs_old/index.md
+-rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-05-03 09:52:04.000000 spotPython-0.1.1/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.1.1/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.893129 spotPython-0.1.1/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    28141 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/00_spot_doc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/01_spot_intro.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8779 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/02_spot_multidim.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/03_spot_anisotropic.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/04_spot_sklearn_surrogate.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/05_spot_sklearn_optimizers.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/06_spot_gaussian.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/07_spot_ei.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/08_spot_noisy.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 06:28:53.000000 spotPython-0.1.1/notebooks/09_spot_ocba.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   125632 2023-05-11 13:54:57.000000 spotPython-0.1.1/notebooks/10_spot_hpt_sklearn_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   293194 2023-05-15 06:49:11.000000 spotPython-0.1.1/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    53313 2023-05-03 09:52:04.000000 spotPython-0.1.1/notebooks/12_spot_hpt_torch_720.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   163882 2023-05-15 06:49:11.000000 spotPython-0.1.1/notebooks/12_spot_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   289738 2023-05-15 06:49:11.000000 spotPython-0.1.1/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   175905 2023-05-18 16:16:45.000000 spotPython-0.1.1/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1150881 2023-05-15 06:49:11.000000 spotPython-0.1.1/notebooks/14_spot_ray_hpt_torch_cifar10_360.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   736654 2023-05-18 11:17:01.000000 spotPython-0.1.1/notebooks/14_spot_ray_hpt_torch_cifar10_720_maans05.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    26701 2023-05-09 10:00:59.000000 spotPython-0.1.1/notebooks/15_spot_hpt_sklearn_regression.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36248 2023-05-18 15:59:41.000000 spotPython-0.1.1/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.850062 spotPython-0.1.1/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.893734 spotPython-0.1.1/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-15 06:49:11.000000 spotPython-0.1.1/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-22 09:13:51.000000 spotPython-0.1.1/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.895423 spotPython-0.1.1/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.1.1/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.1.1/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.1.1/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    38438 2023-04-18 07:53:06.000000 spotPython-0.1.1/notebooks/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-18 13:20:29.000000 spotPython-0.1.1/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-18 16:33:28.906732 spotPython-0.1.1/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.850317 spotPython-0.1.1/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.895887 spotPython-0.1.1/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-18 16:33:28.000000 spotPython-0.1.1/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.896767 spotPython-0.1.1/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-02-02 22:52:12.000000 spotPython-0.1.1/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.897119 spotPython-0.1.1/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-18 07:53:06.000000 spotPython-0.1.1/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.1.1/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.898415 spotPython-0.1.1/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-25 06:56:48.000000 spotPython-0.1.1/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-25 06:56:48.000000 spotPython-0.1.1/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20734 2023-05-11 13:54:57.000000 spotPython-0.1.1/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-25 06:56:48.000000 spotPython-0.1.1/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6169 2023-05-18 14:04:42.000000 spotPython-0.1.1/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-05-03 09:52:04.000000 spotPython-0.1.1/src/spotPython/data/torch_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.898877 spotPython-0.1.1/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.1.1/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.1.1/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-25 06:56:48.000000 spotPython-0.1.1/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.899309 spotPython-0.1.1/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     4163 2023-05-11 13:54:57.000000 spotPython-0.1.1/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4758 2023-05-15 06:49:11.000000 spotPython-0.1.1/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-08 06:28:53.000000 spotPython-0.1.1/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.899606 spotPython-0.1.1/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-31 14:57:36.000000 spotPython-0.1.1/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26028 2023-05-08 06:28:53.000000 spotPython-0.1.1/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.899907 spotPython-0.1.1/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-02-02 22:52:12.000000 spotPython-0.1.1/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-04-25 06:56:48.000000 spotPython-0.1.1/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.900051 spotPython-0.1.1/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    32443 2023-05-15 06:49:11.000000 spotPython-0.1.1/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.900597 spotPython-0.1.1/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)      988 2023-05-18 13:42:35.000000 spotPython-0.1.1/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      401 2023-05-18 13:36:46.000000 spotPython-0.1.1/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      779 2023-05-18 13:42:35.000000 spotPython-0.1.1/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)    15397 2023-05-18 16:33:14.000000 spotPython-0.1.1/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.902234 spotPython-0.1.1/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-11 08:22:02.000000 spotPython-0.1.1/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-15 06:49:11.000000 spotPython-0.1.1/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-18 07:53:06.000000 spotPython-0.1.1/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1415 2023-05-11 13:54:57.000000 spotPython-0.1.1/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-08 06:28:53.000000 spotPython-0.1.1/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-11 13:54:57.000000 spotPython-0.1.1/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)      461 2023-05-03 09:52:04.000000 spotPython-0.1.1/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)      990 2023-05-18 13:19:16.000000 spotPython-0.1.1/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3402 2023-05-11 13:54:57.000000 spotPython-0.1.1/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-18 07:53:06.000000 spotPython-0.1.1/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-18 07:53:06.000000 spotPython-0.1.1/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-11 13:54:57.000000 spotPython-0.1.1/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.896578 spotPython-0.1.1/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     3718 2023-05-18 16:33:28.000000 spotPython-0.1.1/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     7077 2023-05-18 16:33:28.000000 spotPython-0.1.1/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-18 16:33:28.000000 spotPython-0.1.1/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-18 16:33:28.000000 spotPython-0.1.1/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-18 16:33:28.000000 spotPython-0.1.1/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-18 16:33:28.906242 spotPython-0.1.1/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-11 08:22:02.000000 spotPython-0.1.1/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-11 08:22:02.000000 spotPython-0.1.1/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-11 08:22:02.000000 spotPython-0.1.1/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.1.1/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-02-01 14:33:52.000000 spotPython-0.1.1/tox.ini
```

### Comparing `spotPython-0.1.0/.github/workflows/test.yml` & `spotPython-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/.gitignore` & `spotPython-0.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -156,7 +156,8 @@
 Figures.d/10-sklearn_bartz09_5min_20init_2023-05-10_00-43-18_contour_2_3.pdf
 Figures.d/10-sklearn_bartz09_5min_20init_2023-05-10_00-43-18_importance.pdf
 Figures.d/10-sklearn_bartz09_5min_20init_2023-05-10_00-43-18_progress.pdf
 *.pkl
 notebooks/besttorch_model.pt
 notebooks/model_spot_trained.pt
 notebooks/torch_model.pt
+notebooks/model_default_trained.pt
```

### Comparing `spotPython-0.1.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.1.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.1.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.1.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.1.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.1.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.1.1/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/LICENSE.txt` & `spotPython-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/PKG-INFO` & `spotPython-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.1.0
+Version: 0.1.1
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.1.0/README.md` & `spotPython-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/docs/about.md` & `spotPython-0.1.1/docs_old/about.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/docs/examples.md` & `spotPython-0.1.1/docs_old/examples.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/docs/gen_ref_pages.py` & `spotPython-0.1.1/docs_old/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/docs/images/favicon.png` & `spotPython-0.1.1/docs_old/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/docs/images/spotlogo.png` & `spotPython-0.1.1/docs_old/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/00_spot_doc.ipynb` & `spotPython-0.1.1/notebooks/00_spot_doc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/01_spot_intro.ipynb` & `spotPython-0.1.1/notebooks/01_spot_intro.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/02_spot_multidim.ipynb` & `spotPython-0.1.1/notebooks/02_spot_multidim.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/03_spot_anisotropic.ipynb` & `spotPython-0.1.1/notebooks/03_spot_anisotropic.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/04_spot_sklearn_surrogate.ipynb` & `spotPython-0.1.1/notebooks/04_spot_sklearn_surrogate.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/05_spot_sklearn_optimizers.ipynb` & `spotPython-0.1.1/notebooks/05_spot_sklearn_optimizers.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/06_spot_gaussian.ipynb` & `spotPython-0.1.1/notebooks/06_spot_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/07_spot_ei.ipynb` & `spotPython-0.1.1/notebooks/07_spot_ei.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/08_spot_noisy.ipynb` & `spotPython-0.1.1/notebooks/08_spot_noisy.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/09_spot_ocba.ipynb` & `spotPython-0.1.1/notebooks/09_spot_ocba.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/10_spot_hpt_sklearn_classification.ipynb` & `spotPython-0.1.1/notebooks/10_spot_hpt_sklearn_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb` & `spotPython-0.1.1/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/12_spot_hpt_torch_720.ipynb` & `spotPython-0.1.1/notebooks/12_spot_hpt_torch_720.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/12_spot_hpt_torch_cifar10.ipynb` & `spotPython-0.1.1/notebooks/12_spot_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb` & `spotPython-0.1.1/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/14_spot_ray_hpt_torch_cifar10_360.ipynb` & `spotPython-0.1.1/notebooks/14_spot_ray_hpt_torch_cifar10_360.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/15_spot_hpt_sklearn_regression.ipynb` & `spotPython-0.1.1/notebooks/15_spot_hpt_sklearn_regression.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb` & `spotPython-0.1.1/notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.1.1/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/figures/spotModel.graffle` & `spotPython-0.1.1/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/figures/spotModel.pdf` & `spotPython-0.1.1/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/figures/spotModel.png` & `spotPython-0.1.1/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/notebooks/plot.png` & `spotPython-0.1.1/notebooks/plot.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/pyproject.toml` & `spotPython-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.1.0/src/spotPython/budget/ocba.py` & `spotPython-0.1.1/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/build/kriging.py` & `spotPython-0.1.1/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/data/base.py` & `spotPython-0.1.1/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.1.1/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/design/spacefilling.py` & `spotPython-0.1.1/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/fun/hypersklearn.py` & `spotPython-0.1.1/src/spotPython/fun/hypersklearn.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/fun/hypertorch.py` & `spotPython-0.1.1/src/spotPython/fun/hypertorch.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.1.1/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.1.1/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/hyperparameters/values.py` & `spotPython-0.1.1/src/spotPython/hyperparameters/values.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/plot/contour.py` & `spotPython-0.1.1/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/plot/validation.py` & `spotPython-0.1.1/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/spot/spot.py` & `spotPython-0.1.1/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/torch/traintest.py` & `spotPython-0.1.1/src/spotPython/torch/traintest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 from sklearn.model_selection import KFold
 import torch
-from torch import nn
-import torch.optim as optim
+from torch import nn as nn
 from spotPython.utils.device import getDevice
 from torch.utils.data import random_split
 from spotPython.utils.classes import get_additional_attributes
 
 
 def remove_attributes(net, atttributes_to_remove):
     for attr in atttributes_to_remove:
@@ -73,27 +72,31 @@
     k_folds=None,
     show_batch_interval=10_000,
 ):
     lr = net.lr
     epochs = net.epochs
     batch_size = net.batch_size
     k_folds = net.k_folds
+    criterion_instance = net.criterion
+    optimizer_instance = net.optimizer
     removed_attributes = get_additional_attributes(net)
     net = remove_attributes(net, removed_attributes)
     results = {}
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
-        criterion = nn.CrossEntropyLoss()
-        optimizer = optim.Adam(net.parameters(), lr=lr)
+        # criterion = nn.CrossEntropyLoss()
+        # optimizer = optim.Adam(net.parameters(), lr=lr)
+        optimizer = optimizer_instance(net.parameters(), lr=lr)
+        criterion = criterion_instance
         kfold = KFold(n_splits=k_folds, shuffle=shuffle)
         for fold, (train_ids, val_ids) in enumerate(kfold.split(dataset)):
             print(f"Fold: {fold + 1}")
             train_subsampler = torch.utils.data.SubsetRandomSampler(train_ids)
             val_subsampler = torch.utils.data.SubsetRandomSampler(val_ids)
             trainloader = torch.utils.data.DataLoader(
                 dataset, batch_size=batch_size, sampler=train_subsampler, num_workers=num_workers
@@ -112,37 +115,43 @@
         print(f"Error in Net_Core. Call to evaluate_cv() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     net.lr = lr
     net.epochs = epochs
     net.batch_size = batch_size
     net.k_folds = k_folds
+    net.criterion = criterion_instance
+    net.optimizer = optimizer_instance
     return df_eval, df_preds
 
 
 def evaluate_hold_out(
     net, train_dataset, shuffle, test_dataset=None, device=None, show_batch_interval=10_000, path=None, save_model=False
 ):
     lr = net.lr
     epochs = net.epochs
     batch_size = net.batch_size
     patience = net.patience
+    criterion_instance = net.criterion
+    optimizer_instance = net.optimizer
     removed_attributes = get_additional_attributes(net)
     net = remove_attributes(net, removed_attributes)
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
-        criterion = nn.CrossEntropyLoss()
+        # criterion = nn.CrossEntropyLoss()
         # TODO: optimizer = optim.Adam(net.parameters(), lr=lr)
-        optimizer = optim.SGD(net.parameters(), lr=lr, momentum=0.9)
+        # optimizer = optim.SGD(net.parameters(), lr=lr, momentum=0.9)
+        optimizer = optimizer_instance(net.parameters(), lr=lr)
+        criterion = criterion_instance
         if test_dataset is None:
             trainloader, valloader = create_train_val_data_loaders(
                 dataset=train_dataset, batch_size=batch_size, shuffle=shuffle
             )
         else:
             trainloader, valloader = create_train_test_data_loaders(
                 dataset=train_dataset, batch_size=batch_size, shuffle=shuffle, test_dataset=test_dataset
@@ -185,14 +194,16 @@
         print(f"Error in Net_Core. Call to evaluate_hold_out() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     net.lr = lr
     net.epochs = epochs
     net.batch_size = batch_size
     net.patience = patience
+    net.criterion = criterion_instance
+    net.optimizer = optimizer_instance
     print(f"Returned to Spot: Validation loss: {df_eval}")
     print("----------------------------------------------")
     return df_eval, df_preds
 
 
 def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
     test_abs = int(len(dataset) * 0.6)
@@ -266,27 +277,31 @@
 
 
 def train_save(net, train_dataset, shuffle, device=None, show_batch_interval=10_000, path=None, save_model=False):
     lr = net.lr
     epochs = net.epochs
     batch_size = net.batch_size
     patience = net.patience
+    criterion_instance = net.criterion
+    optimizer_instance = net.optimizer
     removed_attributes = get_additional_attributes(net)
     net = remove_attributes(net, removed_attributes)
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
-        criterion = nn.CrossEntropyLoss()
+        # criterion = nn.CrossEntropyLoss()
         # TODO: optimizer = optim.Adam(net.parameters(), lr=lr)
-        optimizer = optim.SGD(net.parameters(), lr=lr, momentum=0.9)
+        # optimizer = optim.SGD(net.parameters(), lr=lr, momentum=0.9)
+        optimizer = optimizer_instance(net.parameters(), lr=lr)
+        criterion = criterion_instance
         trainloader, valloader = create_train_val_data_loaders(
             dataset=train_dataset, batch_size=batch_size, shuffle=shuffle
         )
         # TODO: scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=30, gamma=0.1)
         # Early stopping parameters
         patience = patience
         best_val_loss = float("inf")
@@ -325,45 +340,52 @@
         print(f"Error in Net_Core. Call to evaluate_hold_out() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     net.lr = lr
     net.epochs = epochs
     net.batch_size = batch_size
     net.patience = patience
+    net.criterion = criterion_instance
+    net.optimizer = optimizer_instance
     print(f"Returned to Spot: Validation loss: {df_eval}")
     print("----------------------------------------------")
     return df_eval, df_preds
 
 
 def test_saved(net, shuffle, test_dataset=None, device=None, show_batch_interval=10_000, path=None):
     lr = net.lr
     epochs = net.epochs
     batch_size = net.batch_size
     patience = net.patience
+    criterion_instance = net.criterion
+    optimizer_instance = net.optimizer
     removed_attributes = get_additional_attributes(net)
     net = remove_attributes(net, removed_attributes)
     try:
         device = getDevice(device=device)
         if torch.cuda.is_available():
             device = "cuda:0"
             if torch.cuda.device_count() > 1:
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
-        criterion = nn.CrossEntropyLoss()
+        # criterion = nn.CrossEntropyLoss()
+        criterion = criterion_instance
         valloader = torch.utils.data.DataLoader(
             test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=0
         )
         val_accuracy, val_loss = validate_hold_out(net, valloader=valloader, criterion=criterion, device=device)
         df_eval = val_loss
         df_preds = np.nan
     except Exception as err:
         print(f"Error in Net_Core. Call to evaluate_hold_out() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     net.lr = lr
     net.epochs = epochs
     net.batch_size = batch_size
     net.patience = patience
+    net.criterion = criterion_instance
+    net.optimizer = optimizer_instance
     print(f"Returned to Spot: Validation loss: {df_eval}")
     print("----------------------------------------------")
     return df_eval, df_preds
```

### Comparing `spotPython-0.1.0/src/spotPython/utils/aggregate.py` & `spotPython-0.1.1/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/compare.py` & `spotPython-0.1.1/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/convert.py` & `spotPython-0.1.1/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/device.py` & `spotPython-0.1.1/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/eda.py` & `spotPython-0.1.1/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/init.py` & `spotPython-0.1.1/src/spotPython/utils/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,22 +12,24 @@
                 'n_samples': None,
                 'target_column': None,
                 'shuffle': None,
                 'k_folds': None,
                 'device': None}
     """
     fun_control = {
+        "criterion": None,
         "data": None,
         "train": None,
         "test": None,
         "n_samples": None,
         "target_column": None,
         "shuffle": None,
         "eval": None,
         "k_folds": None,
+        "optimizer": None,
         "device": None,
         "metric_params": {},
         "show_batch_interval": 1_000_000,
         "path": None,
         "save_model": False,
     }
     return fun_control
```

### Comparing `spotPython-0.1.0/src/spotPython/utils/metrics.py` & `spotPython-0.1.1/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/progress.py` & `spotPython-0.1.1/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/repair.py` & `spotPython-0.1.1/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython/utils/transform.py` & `spotPython-0.1.1/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.1.1/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.1.0
+Version: 0.1.1
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.1.0/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.1.1/src/spotPython.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.nojekyll
 LICENSE.txt
 MANIFEST.in
 README.md
 makeSpot.sh
 mkdocs.yml
 pyproject.toml
 tox.ini
@@ -39,21 +40,46 @@
 Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
 Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
 Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
-docs/about.md
-docs/download.md
-docs/examples.md
-docs/gen_ref_pages.py
-docs/index.md
-docs/images/favicon.png
-docs/images/spotlogo.png
+docs/bart23e.html
+docs/bart23e.pdf
+docs/index.html
+docs/search.json
+docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_contour_0_2.png
+docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_contour_0_3.png
+docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_contour_2_3.png
+docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_importance.png
+docs/figures/14-torch_bartz09_30min_10init_2023-05-14_14-45-25_progress.png
+docs/figures/parallel.png
+docs/site_libs/bootstrap/bootstrap-icons.css
+docs/site_libs/bootstrap/bootstrap-icons.woff
+docs/site_libs/bootstrap/bootstrap.min.css
+docs/site_libs/bootstrap/bootstrap.min.js
+docs/site_libs/clipboard/clipboard.min.js
+docs/site_libs/quarto-html/anchor.min.js
+docs/site_libs/quarto-html/popper.min.js
+docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+docs/site_libs/quarto-html/quarto.js
+docs/site_libs/quarto-html/tippy.css
+docs/site_libs/quarto-html/tippy.umd.min.js
+docs/site_libs/quarto-nav/quarto-nav.js
+docs/site_libs/quarto-search/autocomplete.umd.js
+docs/site_libs/quarto-search/fuse.min.js
+docs/site_libs/quarto-search/quarto-search.js
+docs_old/about.md
+docs_old/download.md
+docs_old/examples.md
+docs_old/gen_ref_pages.py
+docs_old/index.md
+docs_old/images/favicon.png
+docs_old/images/spotlogo.png
 notebooks/00_spot_doc.ipynb
 notebooks/01_spot_intro.ipynb
 notebooks/02_spot_multidim.ipynb
 notebooks/03_spot_anisotropic.ipynb
 notebooks/04_spot_sklearn_surrogate.ipynb
 notebooks/05_spot_sklearn_optimizers.ipynb
 notebooks/06_spot_gaussian.ipynb
@@ -63,14 +89,15 @@
 notebooks/10_spot_hpt_sklearn_classification.ipynb
 notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
 notebooks/12_spot_hpt_torch_720.ipynb
 notebooks/12_spot_hpt_torch_cifar10.ipynb
 notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
 notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
 notebooks/14_spot_ray_hpt_torch_cifar10_360.ipynb
+notebooks/14_spot_ray_hpt_torch_cifar10_720_maans05.ipynb
 notebooks/15_spot_hpt_sklearn_regression.ipynb
 notebooks/16_spot_hpt_sklearn_multiclass_classification.ipynb
 notebooks/data.json
 notebooks/plot.png
 notebooks/data/torch/model_spot_trained.pt
 notebooks/figures/spotModel.graffle
 notebooks/figures/spotModel.pdf
```

### Comparing `spotPython-0.1.0/test/test_aggregate_mean_var.py` & `spotPython-0.1.1/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_build_Psi.py` & `spotPython-0.1.1/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_build_U.py` & `spotPython-0.1.1/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_build_psi_vec.py` & `spotPython-0.1.1/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_evaluate_new_X.py` & `spotPython-0.1.1/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_evaluate_new_solutions.py` & `spotPython-0.1.1/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_extract_from_bounds.py` & `spotPython-0.1.1/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_generate_design.py` & `spotPython-0.1.1/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_infill.py` & `spotPython-0.1.1/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_nat_to_cod.py` & `spotPython-0.1.1/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_nat_to_cod_init.py` & `spotPython-0.1.1/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_ocba.py` & `spotPython-0.1.1/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_repair_non_numeric.py` & `spotPython-0.1.1/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_set_de_bounds.py` & `spotPython-0.1.1/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_show_progress.py` & `spotPython-0.1.1/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_suggest_new_X.py` & `spotPython-0.1.1/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.1.0/test/test_update_surrogate.py` & `spotPython-0.1.1/test/test_update_surrogate.py`

 * *Files identical despite different names*

