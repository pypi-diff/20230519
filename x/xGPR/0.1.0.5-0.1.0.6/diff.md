# Comparing `tmp/xGPR-0.1.0.5.tar.gz` & `tmp/xGPR-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xGPR-0.1.0.5.tar", last modified: Fri Apr 14 20:37:04 2023, max compression
+gzip compressed data, was "xGPR-0.1.0.6.tar", last modified: Fri May 19 20:08:50 2023, max compression
```

## Comparing `xGPR-0.1.0.5.tar` & `xGPR-0.1.0.6.tar`

### file list

```diff
@@ -1,156 +1,155 @@
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.881173 xGPR-0.1.0.5/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/LICENSE
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-04-14 20:37:04.881173 xGPR-0.1.0.5/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/README.md
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-04-14 20:37:04.881173 xGPR-0.1.0.5/setup.cfg
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9096 2023-03-15 23:06:59.000000 xGPR-0.1.0.5/setup.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.581181 xGPR-0.1.0.5/xGPR/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-04-14 20:36:46.000000 xGPR-0.1.0.5/xGPR/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.597181 xGPR-0.1.0.5/xGPR/cg_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/cg_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/cg_toolkit/cg_linear_operators.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/cg_toolkit/cg_tools.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/cg_toolkit/cuda_cg_linear_operators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.597181 xGPR-0.1.0.5/xGPR/constants/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/constants/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/constants/constants.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.617180 xGPR-0.1.0.5/xGPR/data_handling/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/data_handling/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/data_handling/data_handling_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12408 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/data_handling/dataset_builder.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/data_handling/minibatch_data_handler.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/data_handling/offline_data_handling.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6584 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/data_handling/online_data_handling.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.649180 xGPR-0.1.0.5/xGPR/fitting_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/fitting_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/fitting_toolkit/ams_grad_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/fitting_toolkit/cg_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2633 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/fitting_toolkit/exact_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.677179 xGPR-0.1.0.5/xGPR/kernels/
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.697178 xGPR-0.1.0.5/xGPR/kernels/ARD_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/ARD_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13753 2023-03-20 17:16:47.000000 xGPR-0.1.0.5/xGPR/kernels/ARD_kernels/graph_mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13671 2023-03-20 16:10:39.000000 xGPR-0.1.0.5/xGPR/kernels/ARD_kernels/mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      842 2023-04-05 20:19:07.000000 xGPR-0.1.0.5/xGPR/kernels/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.721177 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/matern.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7309 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/polynomial.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8549 2023-03-28 01:13:00.000000 xGPR-0.1.0.5/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.729177 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8357 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10972 2023-03-15 23:05:25.000000 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/fht_conv1d.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7436 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/graph_polysum.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8425 2023-03-30 18:51:11.000000 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/graph_rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11144 2023-03-30 18:48:28.000000 xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/graph_rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.0.5/xGPR/kernels/kernel_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6327 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/kernels/srht_compressor.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.757176 xGPR-0.1.0.5/xGPR/optimizers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/optimizers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/optimizers/bayes_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/optimizers/crude_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/optimizers/lb_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/optimizers/map_loss_bayes_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/optimizers/pure_bayes_optimizer.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.773176 xGPR-0.1.0.5/xGPR/preconditioners/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/preconditioners/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.0.5/xGPR/preconditioners/inter_device_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/preconditioners/rand_nys_constructors.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/preconditioners/rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/preconditioners/tuning_preconditioners.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.773176 xGPR-0.1.0.5/xGPR/random_feature_generation/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.789176 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.789176 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    29468 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1912 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.809175 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15871 2023-04-05 18:15:36.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1944 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11168 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      937 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    36132 2023-04-05 17:52:01.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2968 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16360 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16951 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17034 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_float.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18168 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23468 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      448 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.825175 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21983 2023-04-05 18:50:58.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2512 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21692 2023-04-05 18:50:50.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2476 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.845174 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15638 2023-03-23 01:10:07.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1167 2023-03-23 01:10:55.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15603 2023-03-23 01:10:28.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1716 2023-03-23 01:10:42.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.865174 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.869174 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12346 2023-04-07 18:12:07.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      526 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12098 2023-04-07 18:12:18.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      519 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.869174 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7794 2023-04-05 18:26:30.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6212 2023-03-29 20:57:59.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      430 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20845 2023-04-05 17:43:25.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1349 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13003 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20206 2023-03-29 21:53:08.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20713 2023-03-29 21:53:03.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21147 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27262 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      454 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
--rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      993 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.873174 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11209 2023-04-07 18:13:06.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      890 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11056 2023-04-07 18:13:14.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      878 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.0.5/xGPR/regression_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.877173 xGPR-0.1.0.5/xGPR/scoring_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/scoring_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/scoring_toolkit/approximate_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/scoring_toolkit/cho_solvers.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/scoring_toolkit/exact_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/scoring_toolkit/nmll_gradient_tools.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/scoring_toolkit/probe_generators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.877173 xGPR-0.1.0.5/xGPR/static_layers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/static_layers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.0.5/xGPR/static_layers/fast_conv.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.877173 xGPR-0.1.0.5/xGPR/tuning_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/tuning_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/tuning_toolkit/direct_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/tuning_toolkit/hparam_scoring.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.881173 xGPR-0.1.0.5/xGPR/visualization_tools/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.0.5/xGPR/visualization_tools/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.0.5/xGPR/visualization_tools/kernel_xpca.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54098 2023-04-05 20:15:14.000000 xGPR-0.1.0.5/xGPR/xGP_Regression.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:37:04.589181 xGPR-0.1.0.5/xGPR.egg-info/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-04-14 20:37:04.000000 xGPR-0.1.0.5/xGPR.egg-info/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8237 2023-04-14 20:37:04.000000 xGPR-0.1.0.5/xGPR.egg-info/SOURCES.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-04-14 20:37:04.000000 xGPR-0.1.0.5/xGPR.egg-info/dependency_links.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-04-14 20:37:04.000000 xGPR-0.1.0.5/xGPR.egg-info/requires.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-04-14 20:37:04.000000 xGPR-0.1.0.5/xGPR.egg-info/top_level.txt
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/LICENSE
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/README.md
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/setup.cfg
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9096 2023-03-15 23:06:59.000000 xGPR-0.1.0.6/setup.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.220004 xGPR-0.1.0.6/xGPR/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-05-19 17:54:39.000000 xGPR-0.1.0.6/xGPR/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.224004 xGPR-0.1.0.6/xGPR/cg_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/cg_linear_operators.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/cg_tools.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.224004 xGPR-0.1.0.6/xGPR/constants/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/constants/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/constants/constants.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.224004 xGPR-0.1.0.6/xGPR/data_handling/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/data_handling_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12408 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/dataset_builder.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/minibatch_data_handler.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/offline_data_handling.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6584 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/data_handling/online_data_handling.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.228004 xGPR-0.1.0.6/xGPR/fitting_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/ams_grad_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2633 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.228004 xGPR-0.1.0.6/xGPR/kernels/
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.228004 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13753 2023-03-20 17:16:47.000000 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/graph_mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13671 2023-03-20 16:10:39.000000 xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      752 2023-05-19 19:50:16.000000 xGPR-0.1.0.6/xGPR/kernels/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.232004 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3718 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3151 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/matern.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7309 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/polynomial.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1796 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11082 2023-03-30 18:48:37.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf_linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8549 2023-03-28 01:13:00.000000 xGPR-0.1.0.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.232004 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8357 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10972 2023-03-15 23:05:25.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/fht_conv1d.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7436 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_polysum.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8425 2023-03-30 18:51:11.000000 xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14864 2023-03-30 15:55:38.000000 xGPR-0.1.0.6/xGPR/kernels/kernel_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6327 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/kernels/srht_compressor.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.236004 xGPR-0.1.0.6/xGPR/optimizers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/bayes_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/crude_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/lb_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/optimizers/map_loss_bayes_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/optimizers/pure_bayes_optimizer.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.236004 xGPR-0.1.0.6/xGPR/preconditioners/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.0.6/xGPR/preconditioners/inter_device_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_constructors.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/preconditioners/tuning_preconditioners.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.236004 xGPR-0.1.0.6/xGPR/random_feature_generation/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.240004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.240004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    29468 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1912 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.244004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15871 2023-04-05 18:15:36.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1944 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11168 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      937 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    36132 2023-04-05 17:52:01.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2968 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16360 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16951 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17034 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_float.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18168 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23468 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      448 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.244004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21983 2023-04-05 18:50:58.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2512 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21692 2023-04-05 18:50:50.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2476 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.248004 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15638 2023-03-23 01:10:07.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1167 2023-03-23 01:10:55.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15603 2023-03-23 01:10:28.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1716 2023-03-23 01:10:42.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.248004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.248004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12346 2023-04-07 18:12:07.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      526 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12098 2023-04-07 18:12:18.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      519 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7794 2023-04-05 18:26:30.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6212 2023-03-29 20:57:59.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      430 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20845 2023-04-05 17:43:25.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1349 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13003 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20206 2023-03-29 21:53:08.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    20713 2023-03-29 21:53:03.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21147 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27262 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      454 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
+-rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      993 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11209 2023-04-07 18:13:06.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      890 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11056 2023-04-07 18:13:14.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      878 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27652 2023-04-05 19:56:01.000000 xGPR-0.1.0.6/xGPR/regression_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/scoring_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/cho_solvers.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5699 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/exact_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/nmll_gradient_tools.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/scoring_toolkit/probe_generators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.252004 xGPR-0.1.0.6/xGPR/static_layers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/static_layers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9825 2023-03-15 23:05:26.000000 xGPR-0.1.0.6/xGPR/static_layers/fast_conv.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/xGPR/tuning_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/tuning_toolkit/hparam_scoring.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.256004 xGPR-0.1.0.6/xGPR/visualization_tools/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.0.6/xGPR/visualization_tools/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.0.6/xGPR/visualization_tools/kernel_xpca.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54098 2023-04-05 20:15:14.000000 xGPR-0.1.0.6/xGPR/xGP_Regression.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-05-19 20:08:50.220004 xGPR-0.1.0.6/xGPR.egg-info/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/requires.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-05-19 20:08:50.000000 xGPR-0.1.0.6/xGPR.egg-info/top_level.txt
```

### Comparing `xGPR-0.1.0.5/LICENSE` & `xGPR-0.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/PKG-INFO` & `xGPR-0.1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.0.5/README.md` & `xGPR-0.1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/setup.py` & `xGPR-0.1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/cg_toolkit/cg_linear_operators.py` & `xGPR-0.1.0.6/xGPR/cg_toolkit/cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/cg_toolkit/cg_tools.pyx` & `xGPR-0.1.0.6/xGPR/cg_toolkit/cg_tools.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/cg_toolkit/cuda_cg_linear_operators.py` & `xGPR-0.1.0.6/xGPR/cg_toolkit/cuda_cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/constants/constants.py` & `xGPR-0.1.0.6/xGPR/constants/constants.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/data_handling/data_handling_baseclass.py` & `xGPR-0.1.0.6/xGPR/data_handling/data_handling_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/data_handling/dataset_builder.py` & `xGPR-0.1.0.6/xGPR/data_handling/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/data_handling/minibatch_data_handler.py` & `xGPR-0.1.0.6/xGPR/data_handling/minibatch_data_handler.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/data_handling/offline_data_handling.py` & `xGPR-0.1.0.6/xGPR/data_handling/offline_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/data_handling/online_data_handling.py` & `xGPR-0.1.0.6/xGPR/data_handling/online_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/fitting_toolkit/ams_grad_toolkit.py` & `xGPR-0.1.0.6/xGPR/fitting_toolkit/ams_grad_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/fitting_toolkit/cg_fitting_toolkit.py` & `xGPR-0.1.0.6/xGPR/fitting_toolkit/cg_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/fitting_toolkit/exact_fitting_toolkit.py` & `xGPR-0.1.0.6/xGPR/fitting_toolkit/exact_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py` & `xGPR-0.1.0.6/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/fitting_toolkit/sgd_fitting_toolkit.py` & `xGPR-0.1.0.6/xGPR/fitting_toolkit/sgd_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/ARD_kernels/graph_mini_ard.py` & `xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/graph_mini_ard.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/ARD_kernels/mini_ard.py` & `xGPR-0.1.0.6/xGPR/kernels/ARD_kernels/mini_ard.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/__init__.py` & `xGPR-0.1.0.6/xGPR/kernels/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from .basic_kernels.polynomial import Polynomial
 
 from .convolution_kernels.fht_conv1d import FHTConv1d
 from .convolution_kernels.graph_rbf import GraphRBF
 from .convolution_kernels.graph_polysum import GraphPolySum
 
 from .ARD_kernels.mini_ard import MiniARD
-from .ARD_kernels.graph_mini_ard import GraphMiniARD
 
 
 KERNEL_NAME_TO_CLASS = {"RBF":RBF,
         "Matern":Matern,
         "FHTConv1d":FHTConv1d,
         "GraphRBF":GraphRBF,
         "Linear":Linear,
         "Poly":Polynomial,
         "GraphPoly":GraphPolySum,
-        "MiniARD":MiniARD,
-        "GraphMiniARD":GraphMiniARD}
+        "MiniARD":MiniARD}
```

### Comparing `xGPR-0.1.0.5/xGPR/kernels/basic_kernels/linear.py` & `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/basic_kernels/matern.py` & `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/matern.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/basic_kernels/polynomial.py` & `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/polynomial.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/basic_kernels/rbf.py` & `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/basic_kernels/rbf_linear.py` & `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/rbf_linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py` & `xGPR-0.1.0.6/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/conv_feature_extractor.py` & `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/conv_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/fht_conv1d.py` & `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/fht_conv1d.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/graph_polysum.py` & `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_polysum.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/convolution_kernels/graph_rbf.py` & `xGPR-0.1.0.6/xGPR/kernels/convolution_kernels/graph_rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/kernel_baseclass.py` & `xGPR-0.1.0.6/xGPR/kernels/kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/kernels/srht_compressor.py` & `xGPR-0.1.0.6/xGPR/kernels/srht_compressor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/optimizers/bayes_grid_optimizer.py` & `xGPR-0.1.0.6/xGPR/optimizers/bayes_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/optimizers/crude_grid_optimizer.py` & `xGPR-0.1.0.6/xGPR/optimizers/crude_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/optimizers/lb_optimizer.py` & `xGPR-0.1.0.6/xGPR/optimizers/lb_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/optimizers/map_loss_bayes_optimizer.py` & `xGPR-0.1.0.6/xGPR/optimizers/map_loss_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/optimizers/pure_bayes_optimizer.py` & `xGPR-0.1.0.6/xGPR/optimizers/pure_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/preconditioners/cuda_rand_nys_preconditioners.py` & `xGPR-0.1.0.6/xGPR/preconditioners/cuda_rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/preconditioners/inter_device_preconditioners.py` & `xGPR-0.1.0.6/xGPR/preconditioners/inter_device_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/preconditioners/rand_nys_constructors.py` & `xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_constructors.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/preconditioners/rand_nys_preconditioners.py` & `xGPR-0.1.0.6/xGPR/preconditioners/rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/preconditioners/tuning_preconditioners.py` & `xGPR-0.1.0.6/xGPR/preconditioners/tuning_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_double.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_float.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution_float.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/double_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/float_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/double_rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.cu` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.h` & `xGPR-0.1.0.6/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/float_rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/regression_baseclass.py` & `xGPR-0.1.0.6/xGPR/regression_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/scoring_toolkit/approximate_nmll_calcs.py` & `xGPR-0.1.0.6/xGPR/scoring_toolkit/approximate_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/scoring_toolkit/cho_solvers.py` & `xGPR-0.1.0.6/xGPR/scoring_toolkit/cho_solvers.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/scoring_toolkit/exact_nmll_calcs.py` & `xGPR-0.1.0.6/xGPR/scoring_toolkit/exact_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/scoring_toolkit/nmll_gradient_tools.py` & `xGPR-0.1.0.6/xGPR/scoring_toolkit/nmll_gradient_tools.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/scoring_toolkit/probe_generators.py` & `xGPR-0.1.0.6/xGPR/scoring_toolkit/probe_generators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/static_layers/fast_conv.py` & `xGPR-0.1.0.6/xGPR/static_layers/fast_conv.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py` & `xGPR-0.1.0.6/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/tuning_toolkit/direct_fitting_optimizer.py` & `xGPR-0.1.0.6/xGPR/tuning_toolkit/direct_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/tuning_toolkit/hparam_scoring.py` & `xGPR-0.1.0.6/xGPR/tuning_toolkit/hparam_scoring.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/visualization_tools/kernel_xpca.py` & `xGPR-0.1.0.6/xGPR/visualization_tools/kernel_xpca.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR/xGP_Regression.py` & `xGPR-0.1.0.6/xGPR/xGP_Regression.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.0.5/xGPR.egg-info/PKG-INFO` & `xGPR-0.1.0.6/xGPR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.0.5/xGPR.egg-info/SOURCES.txt` & `xGPR-0.1.0.6/xGPR.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/ard_convolution.c
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.c
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.c
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/double_rbf_ops.c
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/float_rbf_ops.c
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/double_array_operations.c
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/float_array_operations.c
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_double.pyx
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution_float.pyx
-/home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
 /home/jlparkinson1/Documents/gp_proteins/xGPR/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
 xGPR/__init__.py
 xGPR/regression_baseclass.py
 xGPR/xGP_Regression.py
 xGPR.egg-info/PKG-INFO
 xGPR.egg-info/SOURCES.txt
 xGPR.egg-info/dependency_links.txt
@@ -56,15 +52,14 @@
 xGPR/kernels/basic_kernels/rbf_linear.py
 xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
 xGPR/kernels/convolution_kernels/__init__.py
 xGPR/kernels/convolution_kernels/conv_feature_extractor.py
 xGPR/kernels/convolution_kernels/fht_conv1d.py
 xGPR/kernels/convolution_kernels/graph_polysum.py
 xGPR/kernels/convolution_kernels/graph_rbf.py
-xGPR/kernels/convolution_kernels/graph_rbf_linear.py
 xGPR/optimizers/__init__.py
 xGPR/optimizers/bayes_grid_optimizer.py
 xGPR/optimizers/crude_grid_optimizer.py
 xGPR/optimizers/lb_optimizer.py
 xGPR/optimizers/map_loss_bayes_optimizer.py
 xGPR/optimizers/pure_bayes_optimizer.py
 xGPR/preconditioners/__init__.py
```

