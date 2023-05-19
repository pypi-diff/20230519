# Comparing `tmp/batchflow-0.8.1.tar.gz` & `tmp/batchflow-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchflow-0.8.1.tar", last modified: Mon Feb 13 11:58:43 2023, max compression
+gzip compressed data, was "batchflow-0.8.1a0.tar", max compression
```

## Comparing `batchflow-0.8.1.tar` & `batchflow-0.8.1a0.tar`

### file list

```diff
@@ -1,160 +1,143 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.721623 batchflow-0.8.1/
--rw-r--r--   0 root         (0) root         (0)    11352 2023-02-13 11:58:34.000000 batchflow-0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6793 2023-02-13 11:58:43.717623 batchflow-0.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5906 2023-02-13 11:58:34.000000 batchflow-0.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.697623 batchflow-0.8.1/batchflow/
--rw-r--r--   0 root         (0) root         (0)     1235 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/_const.py
--rw-r--r--   0 root         (0) root         (0)      249 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/_fake.py
--rwxr-xr-x   0 root         (0) root         (0)     7139 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/base.py
--rwxr-xr-x   0 root         (0) root         (0)    41157 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/batch.py
--rw-r--r--   0 root         (0) root         (0)    45334 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/batch_image.py
--rw-r--r--   0 root         (0) root         (0)     8152 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/components.py
--rw-r--r--   0 root         (0) root         (0)    11909 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/config.py
--rw-r--r--   0 root         (0) root         (0)    13025 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/dataset.py
--rw-r--r--   0 root         (0) root         (0)    19140 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)    22900 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/dsindex.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6082 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/model_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.697623 batchflow-0.8.1/batchflow/models/
--rw-r--r--   0 root         (0) root         (0)       86 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.701623 batchflow-0.8.1/batchflow/models/metrics/
--rw-r--r--   0 root         (0) root         (0)      320 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1947 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/base.py
--rw-r--r--   0 root         (0) root         (0)    17211 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/classify.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/loss.py
--rw-r--r--   0 root         (0) root         (0)     6172 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/regression.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/segment.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/metrics/utils.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/sklearn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.701623 batchflow-0.8.1/batchflow/models/torch/
--rw-r--r--   0 root         (0) root         (0)     1230 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    80626 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/base.py
--rw-r--r--   0 root         (0) root         (0)    26643 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/base_mixins.py
--rw-r--r--   0 root         (0) root         (0)     6068 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.705623 batchflow-0.8.1/batchflow/models/torch/blocks/
--rw-r--r--   0 root         (0) root         (0)      664 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/blocks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23549 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/blocks/attention.py
--rw-r--r--   0 root         (0) root         (0)     7225 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/blocks/core.py
--rw-r--r--   0 root         (0) root         (0)    26202 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/blocks/named_blocks.py
--rw-r--r--   0 root         (0) root         (0)     8016 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/blocks/pyramid.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/blocks/transformer_blocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.705623 batchflow-0.8.1/batchflow/models/torch/callbacks/
--rw-r--r--   0 root         (0) root         (0)      140 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4611 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/callbacks/base.py
--rw-r--r--   0 root         (0) root         (0)     4796 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/callbacks/plateau.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/densenet.py
--rw-r--r--   0 root         (0) root         (0)     6814 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/efficientnet.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/initialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.709622 batchflow-0.8.1/batchflow/models/torch/layers/
--rw-r--r--   0 root         (0) root         (0)      826 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4196 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/activation.py
--rw-r--r--   0 root         (0) root         (0)     6650 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/combine.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/conv.py
--rw-r--r--   0 root         (0) root         (0)    17624 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/conv_complex.py
--rw-r--r--   0 root         (0) root         (0)     6825 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/core.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/hamburger.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/multilayer.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/normalization.py
--rwxr-xr-x   0 root         (0) root         (0)     3682 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/pixel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/pooling.py
--rwxr-xr-x   0 root         (0) root         (0)     2540 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/resize.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/utils.py
--rw-r--r--   0 root         (0) root         (0)     5697 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/layers/wrapper_letters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.709622 batchflow-0.8.1/batchflow/models/torch/losses/
--rw-r--r--   0 root         (0) root         (0)      180 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/losses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6876 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/losses/binary.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/losses/core.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/losses/lovasz.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/losses/multiclass.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/losses/ssim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.709622 batchflow-0.8.1/batchflow/models/torch/modules/
--rw-r--r--   0 root         (0) root         (0)      276 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3637 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/modules/core.py
--rw-r--r--   0 root         (0) root         (0)    14484 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/modules/encoder_decoder.py
--rw-r--r--   0 root         (0) root         (0)     8349 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/modules/loaders.py
--rw-r--r--   0 root         (0) root         (0)     5822 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.709622 batchflow-0.8.1/batchflow/models/torch/optimizers/
--rw-r--r--   0 root         (0) root         (0)       61 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/optimizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5742 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/optimizers/radam.py
--rw-r--r--   0 root         (0) root         (0)     8339 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/repr_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/resnest.py
--rw-r--r--   0 root         (0) root         (0)     9326 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/resnet.py
--rw-r--r--   0 root         (0) root         (0)     5661 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/unet.py
--rw-r--r--   0 root         (0) root         (0)     4463 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/utils.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/torch/vgg.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/models/utils.py
--rw-r--r--   0 root         (0) root         (0)    10162 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/monitor.py
--rw-r--r--   0 root         (0) root         (0)    34811 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/named_expr.py
--rw-r--r--   0 root         (0) root         (0)    23798 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/notifier.py
--rw-r--r--   0 root         (0) root         (0)     9696 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/once_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.713623 batchflow-0.8.1/batchflow/opensets/
--rw-r--r--   0 root         (0) root         (0)      493 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/base.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/cifar.py
--rw-r--r--   0 root         (0) root         (0)     4603 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/coco.py
--rw-r--r--   0 root         (0) root         (0)     7556 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/imagenette.py
--rw-r--r--   0 root         (0) root         (0)     5186 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/mnist.py
--rw-r--r--   0 root         (0) root         (0)     7272 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/opensets/pascal.py
--rwxr-xr-x   0 root         (0) root         (0)    61192 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    10662 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/pipeline_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.713623 batchflow-0.8.1/batchflow/plotter/
--rw-r--r--   0 root         (0) root         (0)       62 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/plotter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/plotter/cmaps.py
--rw-r--r--   0 root         (0) root         (0)    65749 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/plotter/plot.py
--rw-r--r--   0 root         (0) root         (0)    10710 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/plotter/utils.py
--rw-r--r--   0 root         (0) root         (0)     5891 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/profiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.713623 batchflow-0.8.1/batchflow/research/
--rw-r--r--   0 root         (0) root         (0)      358 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10804 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/distributor.py
--rw-r--r--   0 root         (0) root         (0)    28320 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/domain.py
--rw-r--r--   0 root         (0) root         (0)    40018 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/experiment.py
--rwxr-xr-x   0 root         (0) root         (0)     3308 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/named_expr.py
--rw-r--r--   0 root         (0) root         (0)     5444 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/profiler.py
--rw-r--r--   0 root         (0) root         (0)    26085 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/research.py
--rw-r--r--   0 root         (0) root         (0)    17471 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/results.py
--rw-r--r--   0 root         (0) root         (0)    23813 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/storage.py
--rw-r--r--   0 root         (0) root         (0)    14495 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/research/utils.py
--rw-r--r--   0 root         (0) root         (0)    10597 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/run_notebook.py
--rw-r--r--   0 root         (0) root         (0)    22054 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/sampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.717623 batchflow-0.8.1/batchflow/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/apply_parallel_test.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/assemble_test.py
--rw-r--r--   0 root         (0) root         (0)     7250 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/common_index_test.py
--rw-r--r--   0 root         (0) root         (0)    10831 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/components_batch_test.py
--rw-r--r--   0 root         (0) root         (0)     9470 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/components_test.py
--rw-r--r--   0 root         (0) root         (0)    11511 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/config_basic_test.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/config_test.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4001 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/dataset_test.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/datasetindex_test.py
--rw-r--r--   0 root         (0) root         (0)     3402 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/filesindex_test.py
--rw-r--r--   0 root         (0) root         (0)    22255 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/metrics_test.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/model_save_load_test.py
--rw-r--r--   0 root         (0) root         (0)     8101 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/named_expr_test.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/notebooks_test.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/plot_notebooks_test.py
--rw-r--r--   0 root         (0) root         (0)     2349 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/rebatch_test.py
--rw-r--r--   0 root         (0) root         (0)     3955 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/regression_metrics_test.py
--rw-r--r--   0 root         (0) root         (0)    26302 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/research_test.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/save_to_test.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/test_loss_test.py
--rw-r--r--   0 root         (0) root         (0)     5183 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/torch_layers_test.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/torch_models_compile_test.py
--rw-r--r--   0 root         (0) root         (0)     4423 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/tests/torch_models_test.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/utils.py
--rw-r--r--   0 root         (0) root         (0)    12034 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/utils_notebook.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/utils_random.py
--rw-r--r--   0 root         (0) root         (0)     7683 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/utils_telegram.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-02-13 11:58:34.000000 batchflow-0.8.1/batchflow/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 11:58:43.697623 batchflow-0.8.1/batchflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6793 2023-02-13 11:58:43.000000 batchflow-0.8.1/batchflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4690 2023-02-13 11:58:43.000000 batchflow-0.8.1/batchflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-13 11:58:43.000000 batchflow-0.8.1/batchflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-13 11:58:43.000000 batchflow-0.8.1/batchflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2023-02-13 11:58:43.000000 batchflow-0.8.1/batchflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-13 11:58:43.000000 batchflow-0.8.1/batchflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-13 11:58:43.721623 batchflow-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1883 2023-02-13 11:58:34.000000 batchflow-0.8.1/setup.py
+-rw-r--r--   0        0        0    11352 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/LICENSE
+-rw-r--r--   0        0        0     5758 2023-02-27 09:14:17.093317 batchflow-0.8.1a0/README.md
+-rw-r--r--   0        0        0     1391 2023-05-19 11:46:31.165613 batchflow-0.8.1a0/batchflow/__init__.py
+-rw-r--r--   0        0        0     1087 2021-06-04 08:46:56.173421 batchflow-0.8.1a0/batchflow/_const.py
+-rw-r--r--   0        0        0      249 2021-02-09 13:27:23.946505 batchflow-0.8.1a0/batchflow/_fake.py
+-rwxr-xr-x   0        0        0     7139 2022-10-07 10:51:16.578966 batchflow-0.8.1a0/batchflow/base.py
+-rwxr-xr-x   0        0        0    41157 2022-10-07 10:51:16.578966 batchflow-0.8.1a0/batchflow/batch.py
+-rw-r--r--   0        0        0    45393 2023-05-19 10:39:31.916652 batchflow-0.8.1a0/batchflow/batch_image.py
+-rw-r--r--   0        0        0     8152 2022-10-07 10:51:16.578966 batchflow-0.8.1a0/batchflow/components.py
+-rw-r--r--   0        0        0    12330 2023-05-18 15:18:41.634740 batchflow-0.8.1a0/batchflow/config.py
+-rw-r--r--   0        0        0    13032 2023-05-18 15:18:41.634740 batchflow-0.8.1a0/batchflow/dataset.py
+-rw-r--r--   0        0        0    19117 2023-05-18 15:18:41.634740 batchflow-0.8.1a0/batchflow/decorators.py
+-rwxr-xr-x   0        0        0    22892 2023-05-18 15:18:41.634740 batchflow-0.8.1a0/batchflow/dsindex.py
+-rw-r--r--   0        0        0      451 2021-02-09 13:27:23.950505 batchflow-0.8.1a0/batchflow/exceptions.py
+-rw-r--r--   0        0        0     6082 2022-10-07 10:51:16.578966 batchflow-0.8.1a0/batchflow/model_dir.py
+-rw-r--r--   0        0        0       86 2020-10-15 15:55:57.405218 batchflow-0.8.1a0/batchflow/models/__init__.py
+-rw-r--r--   0        0        0     1009 2022-02-10 13:38:46.751038 batchflow-0.8.1a0/batchflow/models/base.py
+-rw-r--r--   0        0        0      320 2020-10-15 15:55:57.405218 batchflow-0.8.1a0/batchflow/models/metrics/__init__.py
+-rwxr-xr-x   0        0        0     1947 2020-10-15 15:55:57.405218 batchflow-0.8.1a0/batchflow/models/metrics/base.py
+-rw-r--r--   0        0        0    17219 2023-02-27 09:14:17.097317 batchflow-0.8.1a0/batchflow/models/metrics/classify.py
+-rw-r--r--   0        0        0     1134 2020-10-15 15:55:57.405218 batchflow-0.8.1a0/batchflow/models/metrics/loss.py
+-rw-r--r--   0        0        0     6172 2020-10-15 15:55:57.405218 batchflow-0.8.1a0/batchflow/models/metrics/regression.py
+-rw-r--r--   0        0        0     5581 2020-10-15 15:55:57.405218 batchflow-0.8.1a0/batchflow/models/metrics/segment.py
+-rw-r--r--   0        0        0     1726 2023-05-18 15:18:41.634740 batchflow-0.8.1a0/batchflow/models/metrics/utils.py
+-rw-r--r--   0        0        0     3097 2020-11-25 11:46:34.988937 batchflow-0.8.1a0/batchflow/models/sklearn.py
+-rw-r--r--   0        0        0     3494 2022-07-08 10:28:56.625784 batchflow-0.8.1a0/batchflow/models/torch/README.md
+-rw-r--r--   0        0        0     1230 2023-02-21 08:16:07.998592 batchflow-0.8.1a0/batchflow/models/torch/__init__.py
+-rwxr-xr-x   0        0        0    82485 2023-05-19 10:39:31.916652 batchflow-0.8.1a0/batchflow/models/torch/base.py
+-rw-r--r--   0        0        0    26643 2022-10-07 10:51:16.578966 batchflow-0.8.1a0/batchflow/models/torch/base_mixins.py
+-rw-r--r--   0        0        0     6068 2022-10-07 10:51:16.578966 batchflow-0.8.1a0/batchflow/models/torch/benchmark.py
+-rw-r--r--   0        0        0      664 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/blocks/__init__.py
+-rw-r--r--   0        0        0    23549 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/blocks/attention.py
+-rw-r--r--   0        0        0     7225 2022-07-08 10:28:56.625784 batchflow-0.8.1a0/batchflow/models/torch/blocks/core.py
+-rw-r--r--   0        0        0    26202 2023-02-27 09:14:17.097317 batchflow-0.8.1a0/batchflow/models/torch/blocks/named_blocks.py
+-rw-r--r--   0        0        0     8050 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/blocks/pyramid.py
+-rw-r--r--   0        0        0     3035 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/blocks/transformer_blocks.py
+-rw-r--r--   0        0        0      140 2021-02-09 13:27:23.950505 batchflow-0.8.1a0/batchflow/models/torch/callbacks/__init__.py
+-rw-r--r--   0        0        0     4647 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/callbacks/base.py
+-rw-r--r--   0        0        0     4796 2021-02-09 13:27:23.950505 batchflow-0.8.1a0/batchflow/models/torch/callbacks/plateau.py
+-rw-r--r--   0        0        0     3595 2022-07-08 10:28:56.625784 batchflow-0.8.1a0/batchflow/models/torch/densenet.py
+-rw-r--r--   0        0        0     6814 2022-07-08 10:28:56.625784 batchflow-0.8.1a0/batchflow/models/torch/efficientnet.py
+-rw-r--r--   0        0        0      636 2021-12-15 08:38:36.227293 batchflow-0.8.1a0/batchflow/models/torch/initialization.py
+-rw-r--r--   0        0        0      826 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/__init__.py
+-rw-r--r--   0        0        0     4196 2022-07-08 10:28:56.625784 batchflow-0.8.1a0/batchflow/models/torch/layers/activation.py
+-rw-r--r--   0        0        0     6650 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/combine.py
+-rw-r--r--   0        0        0     3866 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/conv.py
+-rw-r--r--   0        0        0    17624 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/conv_complex.py
+-rw-r--r--   0        0        0     6824 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/layers/core.py
+-rw-r--r--   0        0        0     4945 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/hamburger.py
+-rw-r--r--   0        0        0    12397 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/multilayer.py
+-rw-r--r--   0        0        0     2511 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/layers/normalization.py
+-rwxr-xr-x   0        0        0     3682 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/models/torch/layers/pixel_shuffle.py
+-rw-r--r--   0        0        0     2700 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/layers/pooling.py
+-rwxr-xr-x   0        0        0     2540 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/layers/resize.py
+-rw-r--r--   0        0        0     2679 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/layers/utils.py
+-rw-r--r--   0        0        0     5697 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/layers/wrapper_letters.py
+-rw-r--r--   0        0        0      180 2020-11-25 11:46:34.988937 batchflow-0.8.1a0/batchflow/models/torch/losses/__init__.py
+-rw-r--r--   0        0        0     6875 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/losses/binary.py
+-rw-r--r--   0        0        0     3779 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/losses/core.py
+-rw-r--r--   0        0        0     5122 2020-11-25 11:46:34.988937 batchflow-0.8.1a0/batchflow/models/torch/losses/lovasz.py
+-rw-r--r--   0        0        0     1202 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/losses/multiclass.py
+-rw-r--r--   0        0        0     3913 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/models/torch/losses/ssim.py
+-rw-r--r--   0        0        0      276 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/modules/__init__.py
+-rw-r--r--   0        0        0     3637 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/modules/core.py
+-rw-r--r--   0        0        0    14484 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/modules/encoder_decoder.py
+-rw-r--r--   0        0        0     8349 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/modules/loaders.py
+-rw-r--r--   0        0        0     5822 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/network.py
+-rw-r--r--   0        0        0       61 2020-10-15 15:55:57.413218 batchflow-0.8.1a0/batchflow/models/torch/optimizers/__init__.py
+-rw-r--r--   0        0        0     5742 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/models/torch/optimizers/radam.py
+-rw-r--r--   0        0        0     8339 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/repr_mixin.py
+-rw-r--r--   0        0        0     1942 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/resnest.py
+-rw-r--r--   0        0        0     9326 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/resnet.py
+-rw-r--r--   0        0        0     5661 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/unet.py
+-rw-r--r--   0        0        0     4463 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/models/torch/utils.py
+-rw-r--r--   0        0        0     2211 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/models/torch/vgg.py
+-rw-r--r--   0        0        0     1277 2021-12-09 16:42:41.260613 batchflow-0.8.1a0/batchflow/models/utils.py
+-rw-r--r--   0        0        0    11506 2023-05-19 10:39:31.916652 batchflow-0.8.1a0/batchflow/monitor.py
+-rw-r--r--   0        0        0    34811 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/named_expr.py
+-rwxr-xr-x   0        0        0    24022 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/notifier.py
+-rw-r--r--   0        0        0     9696 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/once_pipeline.py
+-rw-r--r--   0        0        0      493 2021-12-09 16:42:41.260613 batchflow-0.8.1a0/batchflow/opensets/__init__.py
+-rw-r--r--   0        0        0     2299 2022-02-10 13:38:46.755038 batchflow-0.8.1a0/batchflow/opensets/base.py
+-rw-r--r--   0        0        0     4012 2022-02-10 13:38:46.755038 batchflow-0.8.1a0/batchflow/opensets/cifar.py
+-rw-r--r--   0        0        0     4603 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/opensets/coco.py
+-rw-r--r--   0        0        0     7556 2022-02-10 13:38:46.755038 batchflow-0.8.1a0/batchflow/opensets/imagenette.py
+-rw-r--r--   0        0        0     5186 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/opensets/mnist.py
+-rw-r--r--   0        0        0     7272 2022-02-10 13:38:46.755038 batchflow-0.8.1a0/batchflow/opensets/pascal.py
+-rwxr-xr-x   0        0        0    61491 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/pipeline.py
+-rw-r--r--   0        0        0    10993 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/pipeline_executor.py
+-rw-r--r--   0        0        0      209 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/plotter/__init__.py
+-rw-r--r--   0        0        0      231 2023-01-23 09:45:29.805494 batchflow-0.8.1a0/batchflow/plotter/cmaps.py
+-rw-r--r--   0        0        0    65825 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/plotter/plot.py
+-rw-r--r--   0        0        0    10760 2023-02-27 09:14:17.101317 batchflow-0.8.1a0/batchflow/plotter/utils.py
+-rw-r--r--   0        0        0     6388 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/profiler.py
+-rw-r--r--   0        0        0      358 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/research/__init__.py
+-rw-r--r--   0        0        0    10804 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/research/distributor.py
+-rw-r--r--   0        0        0    28308 2023-05-18 15:18:41.638741 batchflow-0.8.1a0/batchflow/research/domain.py
+-rw-r--r--   0        0        0    40016 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/research/experiment.py
+-rwxr-xr-x   0        0        0     3308 2022-07-08 10:28:56.629784 batchflow-0.8.1a0/batchflow/research/named_expr.py
+-rw-r--r--   0        0        0     5491 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/research/profiler.py
+-rw-r--r--   0        0        0    26092 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/research/research.py
+-rw-r--r--   0        0        0    17455 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/research/results.py
+-rw-r--r--   0        0        0    23930 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/research/storage.py
+-rw-r--r--   0        0        0    14611 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/research/utils.py
+-rw-r--r--   0        0        0    10615 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/run_notebook.py
+-rw-r--r--   0        0        0    22054 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/sampler.py
+-rw-r--r--   0        0        0        0 2020-10-15 15:55:57.413218 batchflow-0.8.1a0/batchflow/tests/__init__.py
+-rw-r--r--   0        0        0     3408 2022-10-07 10:51:16.582966 batchflow-0.8.1a0/batchflow/tests/apply_parallel_test.py
+-rw-r--r--   0        0        0     1364 2020-11-25 11:46:34.992937 batchflow-0.8.1a0/batchflow/tests/assemble_test.py
+-rw-r--r--   0        0        0     7287 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/tests/common_index_test.py
+-rw-r--r--   0        0        0    10831 2021-06-04 08:46:56.189421 batchflow-0.8.1a0/batchflow/tests/components_batch_test.py
+-rw-r--r--   0        0        0     9470 2020-10-15 15:55:57.413218 batchflow-0.8.1a0/batchflow/tests/components_test.py
+-rw-r--r--   0        0        0    11511 2020-10-15 15:55:57.413218 batchflow-0.8.1a0/batchflow/tests/config_basic_test.py
+-rw-r--r--   0        0        0     2860 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/tests/config_test.py
+-rw-r--r--   0        0        0     1208 2022-02-10 13:38:46.759039 batchflow-0.8.1a0/batchflow/tests/conftest.py
+-rw-r--r--   0        0        0     4001 2020-10-15 15:55:57.413218 batchflow-0.8.1a0/batchflow/tests/dataset_test.py
+-rw-r--r--   0        0        0     1629 2020-10-15 15:55:57.417218 batchflow-0.8.1a0/batchflow/tests/datasetindex_test.py
+-rw-r--r--   0        0        0     3439 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/tests/filesindex_test.py
+-rw-r--r--   0        0        0    22255 2022-10-07 10:51:16.586966 batchflow-0.8.1a0/batchflow/tests/metrics_test.py
+-rw-r--r--   0        0        0     6819 2022-02-10 13:38:46.759039 batchflow-0.8.1a0/batchflow/tests/model_save_load_test.py
+-rw-r--r--   0        0        0     8101 2022-10-07 10:51:16.586966 batchflow-0.8.1a0/batchflow/tests/named_expr_test.py
+-rw-r--r--   0        0        0   248883 2023-01-23 09:45:29.809514 batchflow-0.8.1a0/batchflow/tests/notebooks/torch_benchmark.ipynb
+-rw-r--r--   0        0        0    40281 2023-01-23 09:45:29.809514 batchflow-0.8.1a0/batchflow/tests/notebooks/torch_test.ipynb
+-rw-r--r--   0        0        0     2773 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/tests/notebooks_test.py
+-rw-r--r--   0        0        0    28552 2022-10-07 10:51:16.586966 batchflow-0.8.1a0/batchflow/tests/plot_notebooks/data_parse_test.ipynb
+-rw-r--r--   0        0        0     1089 2022-07-08 10:28:56.633784 batchflow-0.8.1a0/batchflow/tests/plot_notebooks_test.py
+-rw-r--r--   0        0        0       81 2020-10-15 15:55:57.417218 batchflow-0.8.1a0/batchflow/tests/pytest.ini
+-rw-r--r--   0        0        0     2349 2021-06-04 08:46:56.189421 batchflow-0.8.1a0/batchflow/tests/rebatch_test.py
+-rw-r--r--   0        0        0     3955 2022-10-07 10:51:16.586966 batchflow-0.8.1a0/batchflow/tests/regression_metrics_test.py
+-rw-r--r--   0        0        0    26373 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/tests/research_test.py
+-rw-r--r--   0        0        0      927 2021-02-09 13:27:23.954505 batchflow-0.8.1a0/batchflow/tests/save_to_test.py
+-rw-r--r--   0        0        0     1559 2022-02-10 13:38:46.759039 batchflow-0.8.1a0/batchflow/tests/test_loss_test.py
+-rw-r--r--   0        0        0     5183 2022-07-08 10:28:56.633784 batchflow-0.8.1a0/batchflow/tests/torch_layers_test.py
+-rw-r--r--   0        0        0     1986 2022-07-08 10:28:56.633784 batchflow-0.8.1a0/batchflow/tests/torch_models_compile_test.py
+-rw-r--r--   0        0        0     4423 2022-02-10 13:38:46.759039 batchflow-0.8.1a0/batchflow/tests/torch_models_test.py
+-rw-r--r--   0        0        0     3233 2021-07-06 11:59:15.547244 batchflow-0.8.1a0/batchflow/utils.py
+-rw-r--r--   0        0        0    12045 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/utils_notebook.py
+-rw-r--r--   0        0        0     3010 2022-10-07 10:51:16.586966 batchflow-0.8.1a0/batchflow/utils_random.py
+-rw-r--r--   0        0        0     7828 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/utils_telegram.py
+-rw-r--r--   0        0        0     5571 2023-05-18 15:18:41.642741 batchflow-0.8.1a0/batchflow/variables.py
+-rw-r--r--   0        0        0     2820 2023-05-19 11:49:18.256267 batchflow-0.8.1a0/pyproject.toml
+-rw-r--r--   0        0        0     7998 1970-01-01 00:00:00.000000 batchflow-0.8.1a0/setup.py
+-rw-r--r--   0        0        0     8512 1970-01-01 00:00:00.000000 batchflow-0.8.1a0/PKG-INFO
```

### Comparing `batchflow-0.8.1/LICENSE` & `batchflow-0.8.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/PKG-INFO` & `batchflow-0.8.1a0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: batchflow
-Version: 0.8.1
-Summary: A framework for fast data processing and ML models training
-Home-page: https://github.com/analysiscenter/batchflow
-Author: Roman Kh at al
-Author-email: rhudor@gmail.com
-License: Apache License 2.0
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-Provides-Extra: nn
-License-File: LICENSE
-
 [![License](https://img.shields.io/github/license/analysiscenter/batchflow.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![Python](https://img.shields.io/badge/python-3.6-blue.svg)](https://python.org)
 [![PyTorch](https://img.shields.io/badge/PyTorch-1.7-orange.svg)](https://pytorch.org)
 [![codecov](https://codecov.io/gh/analysiscenter/batchflow/branch/master/graph/badge.svg)](https://codecov.io/gh/analysiscenter/batchflow)
 [![PyPI](https://badge.fury.io/py/batchflow.svg)](https://badge.fury.io/py/batchflow)
 [![Status](https://github.com/analysiscenter/batchflow/workflows/status/badge.svg)](https://github.com/analysiscenter/batchflow/actions?query=workflow%3Astatus)
 
@@ -102,63 +78,51 @@
 
 > `BatchFlow` module is in the beta stage. Your suggestions and improvements are very welcome.
 
 > `BatchFlow` supports python 3.6 or higher.
 
 ### Stable python package
 
-With modern [pipenv](https://docs.pipenv.org/)
+With [poetry](https://python-poetry.org/)
 ```
-pipenv install batchflow
+poetry add batchflow
 ```
 
 With old-fashioned [pip](https://pip.pypa.io/en/stable/)
 ```
 pip3 install batchflow
 ```
 
 ### Development version
 
-With modern [pipenv](https://docs.pipenv.org/)
+With [poetry](https://python-poetry.org/)
 ```
-pipenv install git+https://github.com/analysiscenter/batchflow.git#egg=batchflow
+poetry add --editable git+https://github.com/analysiscenter/batchflow
 ```
 
 With old-fashioned [pip](https://pip.pypa.io/en/stable/)
 ```
-pip3 install git+https://github.com/analysiscenter/batchflow.git
+pip install --editable git+https://github.com/analysiscenter/batchflow
 ```
 
-After that just import `batchflow`:
-```python
-import batchflow as bf
-```
+### Extras
+Some `batchflow` functions and classed require additional dependencies.
+In order to use that functionality you might need to install `batchflow` with extras (e.g. `batchflow[nn]`):
+
+- image - working with image datasets and plotting
+- nn - for neural networks (includes torch, torchvision, ...)
+- datasets - loading standard datasets (MNIST, CIFAR, ...)
+- profile - performance profiling
+- jupyter - utility functions for notebooks
+- research - multiprocess research
+- telegram - for monitoring pipelines via a telegram bot
+- dev - batchflow development (pylint, pytest, ...)
 
-### Git submodule
-In many cases it might be more convenient to install `batchflow` as a submodule in your project repository than as a python package.
-```
-git submodule add https://github.com/analysiscenter/batchflow.git
-git submodule init
-git submodule update
-```
+You can install several extras at once, like `batchflow[image,nn,research]`.
 
-If your python file is located in another directory, you might need to add a path to `batchflow`:
-```python
-import sys
-sys.path.insert(0, "/path/to/batchflow")
-import batchflow as bf
-```
-
-What is great about using a submodule that every commit in your project can be linked to its own commit of a submodule.
-This is extremely convenient in a fast paced research environment.
-
-Relative import is also possible:
-```python
-from .batchflow import Dataset
-```
 
 ## Projects based on BatchFlow
 - [SeismiQB](https://github.com/gazprom-neft/seismiqb) - ML for seismic interpretation
 - [SeismicPro](https://github.com/gazprom-neft/SeismicPro) - ML for seismic processing
 - [PetroFlow](https://github.com/gazprom-neft/petroflow) - ML for well interpretation
 - [PyDEns](https://github.com/analysiscenter/pydens) - DL Solver for ODE and PDE
 - [RadIO](https://github.com/analysiscenter/radio) - ML for CT imaging
```

### Comparing `batchflow-0.8.1/batchflow/__init__.py` & `batchflow-0.8.1a0/batchflow/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 from .batch_image import ImagesBatch
 from .config import Config
 from .dataset import Dataset
 from .pipeline import Pipeline
 from .monitor import *
 from .notifier import Notifier, notifier
 from .named_expr import NamedExpression, B, L, C, F, V, M, D, R, W, P, PP, I, eval_expr
-from .plotter import plot
 from .dsindex import DatasetIndex, FilesIndex
 from .decorators import action, any_action_failed, mjit, deprecated, apply_parallel
 from .exceptions import SkipBatchException, EmptyBatchSequence, StopPipeline
 from .run_notebook import run_notebook
 from .sampler import Sampler, ConstantSampler, NumpySampler, HistoSampler, ScipySampler
 from .utils import save_data_to, read_data_from
 from .utils_random import make_rng, make_seed_sequence, spawn_seed_sequence
 from .utils_notebook import in_notebook, get_notebook_path, get_notebook_name, pylint_notebook,\
                             get_available_gpus, set_gpus
 from .utils_telegram import TelegramMessage
 
-
-__version__ = '0.8.1'
+from importlib.metadata import version, PackageNotFoundError
+try:
+    __version__ = version('batchflow')
+except PackageNotFoundError:
+    # batchflow cannot be found within batchflow dev env only
+    pass
```

### Comparing `batchflow-0.8.1/batchflow/_const.py` & `batchflow-0.8.1a0/batchflow/_const.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/base.py` & `batchflow-0.8.1a0/batchflow/base.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/batch.py` & `batchflow-0.8.1a0/batchflow/batch.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/batch_image.py` & `batchflow-0.8.1a0/batchflow/batch_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """ Contains Batch classes for images """
 import os
 import warnings
 from numbers import Number
 
 import numpy as np
-import PIL
-import PIL.ImageOps
-import PIL.ImageChops
-import PIL.ImageFilter
-import PIL.ImageEnhance
+try:
+    import PIL
+    import PIL.ImageOps
+    import PIL.ImageChops
+    import PIL.ImageFilter
+    import PIL.ImageEnhance
+except ImportError:
+    pass
+
 from scipy.ndimage.filters import gaussian_filter
 from scipy.ndimage.interpolation import map_coordinates
 
 from .batch import Batch
 from .decorators import action, apply_parallel, inbatch_parallel
 from .dsindex import FilesIndex
 
@@ -856,15 +860,15 @@
         multiplier = np.float32(multiplier)
         if isinstance(image, PIL.Image.Image):
             if preserve_type is False:
                 warnings.warn("Note that some info might be lost during `multiply` transformation since PIL.image "
                               "stores data as `np.uint8`. To suppress this warning, use `preserve_type=True` or "
                               "consider using `to_array` action before multiplication.")
             return PIL.Image.fromarray(np.clip(multiplier*np.asarray(image), 0, 255).astype(np.uint8))
-        dtype = image.dtype if preserve_type else np.float
+        dtype = image.dtype if preserve_type else np.float32
         if clip:
             image = np.clip(multiplier*image, 0, 255 if dtype == np.uint8 else 1.)
         else:
             image = multiplier * image
         return image.astype(dtype)
 
     @apply_parallel
@@ -885,15 +889,15 @@
             Component to write images to. Default is 'images'.
         p : float
             Probability of applying the transform. Default is 1.
         """
         term = np.float32(term)
         if isinstance(image, PIL.Image.Image):
             return PIL.Image.fromarray(np.clip(term+np.asarray(image), 0, 255).astype(np.uint8))
-        dtype = image.dtype if preserve_type else np.float
+        dtype = image.dtype if preserve_type else np.float32
         if clip:
             image = np.clip(term+image, 0, 255 if dtype == np.uint8 else 1.)
         else:
             image = term + image
         return image.astype(dtype)
 
     @apply_parallel
```

### Comparing `batchflow-0.8.1/batchflow/components.py` & `batchflow-0.8.1a0/batchflow/components.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/config.py` & `batchflow-0.8.1a0/batchflow/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
                         val = _config[var_name]
             else:
                 if has_default:
                     val = default
                 else:
                     raise KeyError(f"Key '{variable}' not found")
 
+            val = Config(val) if isinstance(val, (dict, Config.IAddDict)) else val
             ret_vars.append(val)
 
         if unpack:
             ret_vars = ret_vars[0]
         else:
             ret_vars = tuple(ret_vars)
         return ret_vars
@@ -292,14 +293,19 @@
             Returns
             -------
             Pipeline
                 Pipeline object with an updated config
         """
         return other << self
 
+    def __eq__(self, other):
+        self_ = self.flatten() if isinstance(self, Config) else self
+        other_ = Config(other).flatten() if isinstance(other, (dict, Config)) else other
+        return self_.__eq__(other_)
+
     def items(self, flatten=False):
         """ Returns config items
 
         Parameters
         ----------
         flatten : bool
             if False, keys and values will be getted from first level of nested dict, else from the last
@@ -356,21 +362,25 @@
         Parameters
         ----------
         other : dict or Config
 
         kwargs :
             parameters from kwargs also will be included into the resulting config
         """
-        other = dict() if other is None else other
+        other = {} if other is None else other
         if isinstance(other, (dict, Config)):
             for key, value in other.items():
                 self.put(key, value)
         else:
             for key, value in kwargs.items():
                 self.put(key, value)
 
+    def copy(self):
+        """ Create a shallow copy of the instance. """
+        return Config(self.config.copy())
+
     def __iter__(self):
         return iter(self.config)
 
     def __repr__(self):
         lines = ['\n' + 4 * ' ' + line for line in pformat(self.config).split('\n')]
         return f"Config({''.join(lines)})"
```

### Comparing `batchflow-0.8.1/batchflow/dataset.py` & `batchflow-0.8.1a0/batchflow/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,13 +365,13 @@
         for split_size in split_sizes:
             start, stop = current, current + split_size
             splits.append(self.indices[order[start:stop]])
             current = stop
         return splits
 
     def __getstate__(self):
-        return self.__dict__
+        return self.__dict__.copy()
 
     def __setstate__(self, state):
         for k, v in state.items():
             # this warrants that all hidden objects are reconstructed upon unpickling
             setattr(self, k, v)
```

### Comparing `batchflow-0.8.1/batchflow/decorators.py` & `batchflow-0.8.1a0/batchflow/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                     logging.error("Parallel action failed %s", all_errors)
                     traceback.print_tb(all_errors[0].__traceback__)
                     raise RuntimeError("Parallel action failed")
                 return self
             return post_fn(all_results, *args, **kwargs)
 
         def _prepare_args(self, args, kwargs):
-            params = list()
+            params = []
 
             def _get_value(value, pos=None, name=None):
                 if isinstance(value, P):
                     if pos is not None:
                         params.append(pos)
                     elif name is not None:
                         params.append(name)
@@ -297,19 +297,19 @@
 
         def _make_args(self, iteration, init_args, args, kwargs, params=None):
             """ Make args, kwargs tuple """
             if isinstance(init_args, tuple) and len(init_args) == 2 and \
                isinstance(init_args[0], tuple) and isinstance(init_args[1], dict):
                 margs, mkwargs = init_args
             elif isinstance(init_args, dict):
-                margs = list()
+                margs = []
                 mkwargs = init_args
             else:
                 margs = init_args
-                mkwargs = dict()
+                mkwargs = {}
 
             margs = margs if isinstance(margs, (list, tuple)) else [margs]
 
             if params:
                 _args = list(args)
                 _kwargs = {**kwargs}
                 for k in params:
@@ -391,15 +391,15 @@
             args, kwargs, params = _prepare_args(self, args, kwargs)
             full_kwargs = {**dec_kwargs, **kwargs}
 
             for iteration, arg in enumerate(_call_init_fn(init_fn, args, full_kwargs)):
                 margs, mkwargs = _make_args(self, iteration, arg, args, kwargs, params)
                 futures.append(loop.create_task(method(*margs, **mkwargs)))
 
-            loop.run_until_complete(asyncio.gather(*futures, loop=loop, return_exceptions=True))
+            loop.run_until_complete(asyncio.gather(*futures, return_exceptions=True))
 
             return _call_post_fn(self, post_fn, futures, args, full_kwargs)
 
         def wrap_with_for(self, debug, args, kwargs):
             """ Run a method sequentially (without parallelism) """
             init_fn, post_fn = _check_functions(self)
             _ = kwargs.pop('n_workers', _workers_count())
```

### Comparing `batchflow-0.8.1/batchflow/dsindex.py` & `batchflow-0.8.1a0/batchflow/dsindex.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             warnings.warn("Index contains non-unique elements")
 
         return _index
 
     def build_pos(self):
         """ Create a dictionary with positions in the index. """
         if self.indices is None:
-            return dict()
+            return {}
         return dict(zip(self.indices, np.arange(len(self))))
 
     def get_pos(self, index):
         """ Return position of an item in the index.
 
         Parameters
         ----------
@@ -606,15 +606,15 @@
         else:
             paths = path
 
         if len(paths) == 0:
             raise ValueError("`path` must contain at least one entry.")
 
         _all_index = []
-        _all_paths = dict()
+        _all_paths = {}
         for one_path in paths:
             _index, _paths = self.build_from_one_path(one_path, dirs, no_ext)
             _all_index.append(_index)
             _all_paths.update(_paths)
 
         _all_index = np.ravel(_all_index)
```

### Comparing `batchflow-0.8.1/batchflow/model_dir.py` & `batchflow-0.8.1a0/batchflow/model_dir.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/base.py` & `batchflow-0.8.1a0/batchflow/models/base.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/metrics/base.py` & `batchflow-0.8.1a0/batchflow/models/metrics/base.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/metrics/classify.py` & `batchflow-0.8.1a0/batchflow/models/metrics/classify.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from copy import copy
 from functools import partial
 
 import numpy as np
 
 from ...decorators import mjit
 from . import Metrics, binarize, sigmoid, infmean
-from ...plotter import plot
 
 
 
 METRICS_ALIASES = {'sensitivity' : 'true_positive_rate',
                    'recall' : 'true_positive_rate',
                    'tpr' : 'true_positive_rate',
                    'fallout' : 'false_positive_rate',
@@ -188,14 +187,15 @@
             'ytick_locations': np.arange(confusion_matrix.shape[1]),
             'ytick_labels': classes,
             'ytick_rotation': 0,
             'ytick_va': 'center',
             **kwargs
         }
 
+        from ...plotter import plot
         return plot(data=confusion_matrix, mode='matrix', **plot_config)
 
     def copy(self):
         """ Return a duplicate containing only the confusion matrix """
         metrics = copy(self)
         metrics.free()
         return metrics
```

### Comparing `batchflow-0.8.1/batchflow/models/metrics/loss.py` & `batchflow-0.8.1a0/batchflow/models/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/metrics/regression.py` & `batchflow-0.8.1a0/batchflow/models/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/metrics/segment.py` & `batchflow-0.8.1a0/batchflow/models/metrics/segment.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/metrics/utils.py` & `batchflow-0.8.1a0/batchflow/models/metrics/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Contains utility function for metrics evaluation """
 import numpy as np
-import numpy.ma as ma
+from numpy import ma
 try:
     from scipy.ndimage import measurements
 except ImportError:
     pass
 try:
     from numba import njit
 except ImportError:
```

### Comparing `batchflow-0.8.1/batchflow/models/sklearn.py` & `batchflow-0.8.1a0/batchflow/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/__init__.py` & `batchflow-0.8.1a0/batchflow/models/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/base.py` & `batchflow-0.8.1a0/batchflow/models/torch/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from math import ceil
 from threading import Lock
 from functools import partial
 from contextlib import nullcontext
 
 import dill
 import numpy as np
-import pandas as pd
+try:
+    import pandas as pd
+except ImportError:
+    pass
 
 import torch
 from torch import nn
 from torch.optim.swa_utils import AveragedModel, SWALR
 
 try:
     import cupy as cp
@@ -690,15 +693,15 @@
         self.scaler = torch.cuda.amp.GradScaler()
 
         self.setup_gradient_clipping()
         self.setup_weights_averaging()
 
     def unpack(self, value):
         """ Unpack argument to actual value and kwargs. """
-        if isinstance(value, dict):
+        if isinstance(value, (dict, Config)):
             kwargs = value.copy()
             value = kwargs.pop('name', None)
         else:
             kwargs = {}
 
         return value, kwargs
 
@@ -787,19 +790,21 @@
                 raise ValueError('Missing `frequency` key in the decay configuration')
 
             # Set defaults for some of the decays
             if decay_ in DECAYS_DEFAULTS:
                 decay_dict = DECAYS_DEFAULTS.get(decay_).copy()
                 if decay == DECAYS['cos']:
                     decay_dict.update(T_max=step_params['frequency'])
-                decay_kwargs = {**decay_dict, **decay_kwargs}
+                decay_kwargs = Config({**decay_dict, **decay_kwargs})
+            else:
+                decay_kwargs = Config(decay_kwargs)
 
             # Remove unnecessary keys from kwargs
             for key in ['start_iter', 'last_iter', 'frequency']:
-                decay_kwargs.pop(key, None)
+                decay_kwargs.pop(key, default=None)
 
             # Create decay or store parameters for later usage
             decay_ = decay_(self.optimizer, **decay_kwargs)
 
             self.decay.append(decay_)
             self.decay_step.append(step_params)
 
@@ -914,59 +919,65 @@
                     init_weights_function = best_practice_resnet_init
 
                 # Actual weights initialization
                 self.model.apply(init_weights_function)
 
 
     # Transfer to/from device(s)
-    def transfer_to_device(self, data):
+    def transfer_to_device(self, data, non_blocking=False):
         """ Transfer (possibly nested) data structure to device and return the same structure. """
         if isinstance(data, (dict, Config)):
             return type(data)({key : self.transfer_to_device(value) for key, value in data.items()})
 
         if isinstance(data, (tuple, list)):
             return type(data)(self.transfer_to_device(item) for item in data)
 
         if isinstance(data, np.ndarray):
             if data.dtype != np.float32:
                 data = data.astype(np.float32)
             data = torch.from_numpy(data)
 
             if self.config['channels_last'] and data.ndim == 4:
                 data = data.to(memory_format=torch.channels_last)
-            data = data.to(self.device)
+            data = data.to(self.device, non_blocking=non_blocking)
             return data
 
         if isinstance(data, torch.Tensor):
-            data = data.to(self.device)
+            data = data.to(self.device, non_blocking=non_blocking)
             return data
 
         if CUPY_AVAILABLE and isinstance(data, cp.ndarray):
             if data.device.id == self.device.index:
                 data = torch.utils.dlpack.from_dlpack(data.toDlpack())
                 return data
             raise TypeError(f'cupy arrays should reside on the same GPU, as model itself: {self.device}.')
 
         if data is None:
             return None
         raise TypeError('Passed data should either be a `np.ndarray`, `torch.Tensor`, `cupy.ndarray`, '
                         f'or a container of them, got{type(data)}.')
 
-    def transfer_from_device(self, data):
+    def transfer_from_device(self, data, force_float32_dtype=True):
         """ Transfer (possibly nested) data structure from device and return the same structure. """
         if isinstance(data, (dict, Config)):
-            return type(data)({key : self.transfer_from_device(value) for key, value in data.items()})
+            return type(data)({key : self.transfer_from_device(value, force_float32_dtype)
+                               for key, value in data.items()})
 
         if isinstance(data, (tuple, list)):
-            return type(data)(self.transfer_from_device(item) for item in data)
+            return type(data)(self.transfer_from_device(item, force_float32_dtype) for item in data)
 
         if isinstance(data, (torch.Tensor, torch.autograd.Variable)):
+            # cpu_tensor = data.detach().cpu().numpy()
+            # if self.amp and cpu_tensor.dtype != np.float32:
+            #     cpu_tensor = cpu_tensor.astype(np.float32)
+            # return cpu_tensor
+
+            if force_float32_dtype and data.dtype != torch.float32:
+                data = data.float()
             cpu_tensor = data.detach().cpu().numpy()
-            if self.amp and cpu_tensor.dtype != np.float32:
-                cpu_tensor = cpu_tensor.astype(np.float32)
             return cpu_tensor
 
         if isinstance(data, (np.ndarray, int, float)):
             return data
         raise TypeError('Passed data should either be a `np.ndarray`, `torch.Tensor`'
                         f' or a container of them, got {type(data)}.')
 
@@ -979,15 +990,15 @@
         else:
             self.model.to(self.device)
 
 
     # Apply model to train/predict on given data
     def train(self, inputs, targets, outputs=None, mode='train', lock=True, profile=False,
               sync_frequency=True, microbatch_size=None, microbatch_drop_last=True, microbatch_pad_last=False,
-              sam_rho=None, sam_individual_norm=None, transfer_from_device=True):
+              sam_rho=None, sam_individual_norm=None, transfer_from_device=True, force_float32_dtype=True):
         """ Train the model with the data provided
 
         Parameters
         ----------
         inputs : np.ndarray or sequence of them
             Model inputs. If there is a single input, then it is passed to model directly; otherwise, we pass a list.
             If the microbatching is used, individual elements are split along the first axis.
@@ -1024,14 +1035,17 @@
             If True, then each gradient is scaled according to its own L2 norm.
             If False, then one common gradient norm is computed and used as a scaler for all gradients.
         profile : bool
             Whether to collect stats of model training timings.
             If True, then stats can be accessed via `profile_info` attribute or :meth:`.show_profile_info` method.
         transfer_from_device : bool
             Whether to transfer requested `outputs` from device to CPU.
+        force_float32_dtype : bool
+            Whether to force dtype float32 to the model outputs.
+            Otherwise, the dtype is preserved and may be affected by AMP.
 
         Returns
         -------
         Calculated values of requested tensors from `outputs` in the same order.
 
         Examples
         --------
@@ -1041,15 +1055,15 @@
         """
         if self.disable_training:
             raise RuntimeError('Training model after ONNX conversion is not allowed!')
 
         # Lock the entire method; release in any case
         try:
             if lock:
-                self.model_lock.acquire()
+                self.model_lock.acquire() #pylint: disable=consider-using-with
             self.last_train_info = {}
 
             # Parse inputs and targets: always a list
             inputs = list(inputs) if isinstance(inputs, (tuple, list)) else [inputs]
             targets = list(targets) if isinstance(targets, (tuple, list)) else [targets]
 
             # Parse outputs: always a list
@@ -1104,15 +1118,16 @@
             # Train on each of the microbatches
             chunked_outputs = []
             for chunk_inputs, chunk_targets in zip(chunked_inputs, chunked_targets):
                 # Compute forward and backward passes of the model, apply gradients, evaluate requested outputs
                 chunk_outputs = self._train(inputs=chunk_inputs, targets=chunk_targets, outputs=outputs[:],
                                             sync_frequency=sync_frequency*steps,
                                             sam_rho=sam_rho, sam_individual_norm=sam_individual_norm,
-                                            transfer_from_device=transfer_from_device)
+                                            transfer_from_device=transfer_from_device,
+                                            force_float32_dtype=force_float32_dtype)
                 chunked_outputs.append(chunk_outputs)
 
             # Exit the profiling
             if profile:
                 profiler.__exit__(None, None, None)
                 self.profilers.append(profiler)
 
@@ -1154,20 +1169,21 @@
             })
 
         finally:
             if lock:
                 self.model_lock.release()
         return result
 
-    def _train(self, inputs, targets, outputs, sync_frequency, sam_rho, sam_individual_norm, transfer_from_device):
+    def _train(self, inputs, targets, outputs, sync_frequency, sam_rho, sam_individual_norm,
+               transfer_from_device, force_float32_dtype):
         # Parse inputs
         inputs = inputs[0] if len(inputs) == 1 and isinstance(inputs, list) else inputs
         targets = targets[0] if len(targets) == 1 and isinstance(targets, list) else targets
         inputs = self.transfer_to_device(inputs)
-        targets = self.transfer_to_device(targets)
+        targets = self.transfer_to_device(targets, non_blocking=True)
 
         # Convert layer ids into LayerHooks
         outputs = self.prepare_outputs(outputs)
 
         # Compute predictions; store shapes for introspection
         with torch.cuda.amp.autocast(enabled=self.amp):
             predictions = self.model(inputs)
@@ -1238,15 +1254,15 @@
         self.last_train_info['available_outputs'] = list(output_container.keys())
 
         # Retrieve requested outputs
         requested_outputs = self.extract_outputs(outputs, output_container)
 
         # Transfer only the requested outputs to CPU
         if transfer_from_device:
-            requested_outputs = self.transfer_from_device(requested_outputs)
+            requested_outputs = self.transfer_from_device(requested_outputs, force_float32_dtype=force_float32_dtype)
         return requested_outputs
 
     def _train_sam_store_gradients(self):
         """ Store gradients from previous microbatches. """
         for p in self.model.parameters():
             if p.grad is not None:
                 self.optimizer.state[p]['previous_grad'] = p.grad.clone().detach()
@@ -1287,15 +1303,15 @@
         for p in self.model.parameters():
             previous_grad = self.optimizer.state[p].get('previous_grad')
             if previous_grad is not None:
                 p.grad.add_(previous_grad)
 
 
     def predict(self, inputs, targets=None, outputs=None, lock=True, microbatch_size=False, microbatch_pad_last=False,
-                amp=None, mode='eval', no_grad=True, transfer_from_device=True):
+                amp=None, mode='eval', no_grad=True, transfer_from_device=True, force_float32_dtype=True):
         """ Get predictions on the data provided.
 
         Parameters
         ----------
         inputs : np.ndarray or sequence of them
             Model inputs. Passed directly to model.
         targets : np.ndarray or sequence of them
@@ -1318,14 +1334,17 @@
         amp : None or bool
             If None, then use amp setting from config.
             If bool, then overrides the amp setting for prediction.
         no_grad : bool
             Whether to disable gradient computation during model evaluation.
         transfer_from_device : bool
             Whether to transfer requested `outputs` from device to CPU.
+        force_float32_dtype : bool
+            Whether to force dtype float32 to the model outputs.
+            Otherwise, the dtype is preserved and may be affected by AMP.
 
         Returns
         -------
         Calculated values of tensors in `outputs` in the same order.
 
         Examples
         --------
@@ -1341,15 +1360,15 @@
         if self._loaded_from_onnx:
             microbatch_size = self.microbatch_size
             microbatch_pad_last = True
 
         # Acquire lock; release in any case
         try:
             if lock:
-                self.model_lock.acquire()
+                self.model_lock.acquire() #pylint: disable=consider-using-with
             self.last_predict_info = {}
 
             # Parse inputs and targets: always a list
             inputs = list(inputs) if isinstance(inputs, (tuple, list)) else [inputs]
             if targets is not None:
                 targets = (list(targets) if isinstance(targets, (tuple, list)) else [targets])
             else:
@@ -1380,15 +1399,16 @@
             # Evaluate each microbatch separately
             self.set_model_mode(mode)
 
             chunked_outputs = []
             for chunk_inputs, chunk_targets in zip(chunked_inputs, chunked_targets):
                 # Evaluate requested outputs
                 chunk_outputs = self._predict(inputs=chunk_inputs, targets=chunk_targets, outputs=outputs[:],
-                                              amp=amp, no_grad=no_grad, transfer_from_device=transfer_from_device)
+                                              amp=amp, no_grad=no_grad, transfer_from_device=transfer_from_device,
+                                              force_float32_dtype=force_float32_dtype)
                 chunked_outputs.append(chunk_outputs)
 
             # Aggregate the outputs from microbatches
             result = self.aggregate_microbatches(outputs, chunked_outputs, chunk_sizes, single_output)
 
             # Store info about current predict iteration
             self.last_predict_info.update({
@@ -1400,15 +1420,15 @@
             })
 
         finally:
             if lock:
                 self.model_lock.release()
         return result
 
-    def _predict(self, inputs, targets, outputs, amp, no_grad, transfer_from_device):
+    def _predict(self, inputs, targets, outputs, amp, no_grad, transfer_from_device, force_float32_dtype):
         # Parse inputs
         inputs = inputs[0] if len(inputs) == 1 and isinstance(inputs, list) else inputs
         targets = targets[0] if len(targets) == 1 and isinstance(targets, list) else targets
 
         # Convert layer ids into LayerHooks
         outputs = self.prepare_outputs(outputs)
 
@@ -1430,19 +1450,19 @@
 
         # Log inner info
         predictions_ = list(predictions) if isinstance(predictions, (tuple, list)) else [predictions]
         self.last_predict_info['predictions_shapes'] = [get_shape(item) for item in predictions_]
         self.last_predict_info['available_outputs'] = list(output_container.keys())
 
         # Retrieve requested outputs
-        requested_outputs = self.extract_outputs(outputs, output_container)
+        requested_outputs = self.extract_outputs(outputs, output_container, predictions=predictions)
 
         # Transfer only the requested outputs to CPU
         if transfer_from_device:
-            requested_outputs = self.transfer_from_device(requested_outputs)
+            requested_outputs = self.transfer_from_device(requested_outputs, force_float32_dtype=force_float32_dtype)
         return requested_outputs
 
 
     def __call__(self, inputs, targets=None, outputs='predictions', lock=True,
                  microbatch_size=False, microbatch_pad_last=False,
                  amp=False, no_grad=False, transfer_from_device=False):
         """ Evaluate model on provided data, while tracking gradients.
@@ -1579,29 +1599,33 @@
     @staticmethod
     def apply_output_operation(tensor, operation):
         """ Apply `operation`, possibly aliased with a string, to `tensor`. """
         with torch.no_grad():
             if operation is None:
                 result = tensor
                 name = ''
-            elif operation == 'softplus':
-                result = torch.nn.functional.softplus(tensor)
-                name = operation
-            elif operation == 'sigmoid':
-                result = torch.sigmoid(tensor)
-                name = operation
-            elif operation == 'proba':
-                result = torch.nn.functional.softmax(tensor, dim=1)
-                name = operation
-            elif operation == 'labels':
-                result = tensor.argmax(dim=1)
-                name = operation
             elif callable(operation):
                 result = operation(tensor)
                 name = operation.__name__
+            else:
+                if operation == 'softplus':
+                    result = torch.nn.functional.softplus(tensor)
+                elif operation == 'sigmoid':
+                    result = torch.sigmoid(tensor)
+                elif operation == 'sigmoid_uint8':
+                    result = (torch.sigmoid(tensor) * 255).to(dtype=torch.uint8)
+                elif operation == 'sigmoid_int16':
+                    result = (torch.sigmoid(tensor) * 255).to(dtype=torch.int16)
+                elif operation == 'proba':
+                    result = torch.nn.functional.softmax(tensor, dim=1)
+                elif operation == 'labels':
+                    result = tensor.argmax(dim=1)
+                else:
+                    raise ValueError(f'Unknown type of operation `{operation}`!')
+                name = operation
         return result, name
 
 
     def prepare_outputs(self, outputs):
         """ Add the hooks to all outputs that look like a layer id. """
         result = []
         for output_name in outputs:
@@ -1609,23 +1633,25 @@
                 layer = self.get_layer(output_name)
                 hook = LayerHook(layer)
                 result.append(hook)
             else:
                 result.append(output_name)
         return result
 
-    def extract_outputs(self, outputs, output_container):
+    def extract_outputs(self, outputs, output_container, predictions=None):
         """ Retrieve activation data from hooks, get other requested outputs from container. """
         requested_outputs = []
         for item in outputs:
             if isinstance(item, LayerHook):
                 item.close()
                 value = item.activation
-            else:
+            elif item in output_container:
                 value = output_container[item]
+            else:
+                value = self.apply_output_operation(tensor=predictions, operation=item)[0]
 
             requested_outputs.append(value)
         return requested_outputs
 
 
     # Store model
     def save(self, path, use_onnx=False, path_onnx=None, batch_size=None, opset_version=13,
@@ -1700,14 +1726,15 @@
             Module to use for pickling.
         kwargs : dict
             Other keyword arguments, passed directly to :func:`torch.save`.
         """
         self._parse_devices()
         if self.device:
             kwargs['map_location'] = self.device
+        kwargs['map_location'] = 'cpu'
 
         # Load items from disk storage and set them as insance attributes
         checkpoint = torch.load(path, pickle_module=pickle_module, **kwargs)
 
         # `load_config` is a reference to `self.external_config` used to update `config`
         # It is required since `self.external_config` may be overwritten in the cycle below
         load_config = self.external_config
@@ -1785,15 +1812,15 @@
         else:
             columns = ['ncalls', 'CUDA_cumtime', 'CUDA_cumtime_avg']
             if sortby is None:
                 sortby = ('CUDA_cumtime', 'sum') if per_iter is False else 'CUDA_cumtime'
 
         if per_iter is False:
             aggs = {key: ['sum', 'mean', 'max'] for key in columns}
-            result = (self.profile_info.reset_index().groupby(['name']).agg(aggs)
+            result = (self.profile_info.reset_index().groupby(['name']).agg(aggs, numeric_only=True)
                       .sort_values(sortby, ascending=False)[:limit])
         else:
             result = (self.profile_info.reset_index().set_index(['iter', 'name'])[columns]
                       .sort_values(['iter', sortby], ascending=[True, False])
                       .groupby(level=0).apply(lambda df: df[:limit]).droplevel(0))
         return result
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/base_mixins.py` & `batchflow-0.8.1a0/batchflow/models/torch/base_mixins.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/benchmark.py` & `batchflow-0.8.1a0/batchflow/models/torch/benchmark.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/blocks/__init__.py` & `batchflow-0.8.1a0/batchflow/models/torch/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/blocks/attention.py` & `batchflow-0.8.1a0/batchflow/models/torch/blocks/attention.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/blocks/core.py` & `batchflow-0.8.1a0/batchflow/models/torch/blocks/core.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/blocks/named_blocks.py` & `batchflow-0.8.1a0/batchflow/models/torch/blocks/named_blocks.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/blocks/pyramid.py` & `batchflow-0.8.1a0/batchflow/models/torch/blocks/pyramid.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         Dilation rates for branches, default=(6, 12, 18).
     pyramid : int or tuple of int
         Number of image level features in each dimension.
         Default is 2, i.e. 2x2=4 pooling features will be calculated for 2d images,
         and 2x2x2=8 features per 3d item.
         Tuple allows to define several image level features, e.g (2, 3, 4).
     """
+    #pylint: disable=not-callable
     LAYERS = {
         1: nn.functional.conv1d,
         2: nn.functional.conv2d,
         3: nn.functional.conv3d,
     }
 
     def __init__(self, inputs=None, layout='cnad', channels=None, kernel_size=3,
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/blocks/transformer_blocks.py` & `batchflow-0.8.1a0/batchflow/models/torch/blocks/transformer_blocks.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/callbacks/base.py` & `batchflow-0.8.1a0/batchflow/models/torch/callbacks/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import gmtime, strftime
 
 from ....monitor import USSMonitor, GPUMonitor, GPUMemoryMonitor
 
 
 def file_print(path, msg):
     """ Print to a file. """
-    with open(path, 'a+') as f:
+    with open(path, 'a+', encoding='utf-8') as f:
         print(msg, file=f)
 
 
 
 class BaseCallback(ABC):
     """ Base class for callbacks.
 
@@ -31,15 +31,15 @@
         if stream is None:
             return lambda *args: args
 
         if callable(stream):
             return stream
 
         if isinstance(stream, str):
-            with open(stream, 'w') as _:
+            with open(stream, 'w', encoding='utf-8') as _:
                 pass
             return lambda msg: file_print(stream, msg)
         raise TypeError('`Stream` argument must be either None, callable or string.')
 
     def set_model(self, model):
         """ Save reference to the model.
         Depending on the callback, following attribytes may be accessed:
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/callbacks/plateau.py` & `batchflow-0.8.1a0/batchflow/models/torch/callbacks/plateau.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/densenet.py` & `batchflow-0.8.1a0/batchflow/models/torch/densenet.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/efficientnet.py` & `batchflow-0.8.1a0/batchflow/models/torch/efficientnet.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/initialization.py` & `batchflow-0.8.1a0/batchflow/models/torch/initialization.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/__init__.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/activation.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/activation.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/combine.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/combine.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/conv.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/conv.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/conv_complex.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/conv_complex.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/core.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Basic Torch layers. """
 import torch
-import torch.nn as nn
+from torch import nn
 
 from ..utils import get_shape, get_num_dims, safe_eval
 
 
 
 class Flatten(nn.Module):
     """ Flatten input, optionally keeping provided dimensions.
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/hamburger.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/hamburger.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/multilayer.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/multilayer.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/normalization.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Normalization layers. """
 import torch
-import torch.nn as nn
+from torch import nn
 import torch.nn.functional as F
 
 from ..utils import get_num_channels, get_num_dims
 
 
 
 class LayerNorm(nn.Module):
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/pixel_shuffle.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/pixel_shuffle.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/pooling.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/resize.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/resize.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/utils.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/utils.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/layers/wrapper_letters.py` & `batchflow-0.8.1a0/batchflow/models/torch/layers/wrapper_letters.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/losses/binary.py` & `batchflow-0.8.1a0/batchflow/models/torch/losses/binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Losses for binary predictions. """
 import numpy as np
 
 import torch
-import torch.nn as nn
+from torch import nn
 import torch.nn.functional as F
 
 
 
 class BCE(nn.Module):
     """ Binary cross-entropy that allows int/float for `pos_weight`, unlike native PyTorch implementation.
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/losses/core.py` & `batchflow-0.8.1a0/batchflow/models/torch/losses/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Core loss functions """
 import torch
-import torch.nn as nn
+from torch import nn
 
 
 class CrossEntropyLoss(nn.Module):
     """ Custom loss which casts target dtype if needed.
     Additionally, allows string specifiers for `weight` parameter.
 
     Parameters
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/losses/lovasz.py` & `batchflow-0.8.1a0/batchflow/models/torch/losses/lovasz.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/losses/multiclass.py` & `batchflow-0.8.1a0/batchflow/models/torch/losses/multiclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Losses that work with multiclass tasks. """
 import torch
-import torch.nn as nn
+from torch import nn
 import torch.nn.functional as F
 
 
 
 class Dice(nn.Module):
     """ Sørensen-Dice Coefficient as a loss function. Sudre C. et al. "`Generalised Dice overlap as a deep
     learning loss function for highly unbalanced segmentations <https://arxiv.org/abs/1707.03237>`_".
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/losses/ssim.py` & `batchflow-0.8.1a0/batchflow/models/torch/losses/ssim.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Structural similarity as loss function.
 "Image Quality Assessment: From Error Visibility to Structural Similarity" IEEE
 Transactions on Image Processing Vol. 13. No. 4. April 2004.
 """
 from math import exp
 
 import torch
-import torch.nn as nn
+from torch import nn
 import torch.nn.functional as F
 
 
 class SSIM(nn.Module):
     """ Structural similarity between two images.
     Note that images must be grayscale.
```

### Comparing `batchflow-0.8.1/batchflow/models/torch/modules/core.py` & `batchflow-0.8.1a0/batchflow/models/torch/modules/core.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/modules/encoder_decoder.py` & `batchflow-0.8.1a0/batchflow/models/torch/modules/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/modules/loaders.py` & `batchflow-0.8.1a0/batchflow/models/torch/modules/loaders.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/network.py` & `batchflow-0.8.1a0/batchflow/models/torch/network.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/optimizers/radam.py` & `batchflow-0.8.1a0/batchflow/models/torch/optimizers/radam.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/repr_mixin.py` & `batchflow-0.8.1a0/batchflow/models/torch/repr_mixin.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/resnest.py` & `batchflow-0.8.1a0/batchflow/models/torch/resnest.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/resnet.py` & `batchflow-0.8.1a0/batchflow/models/torch/resnet.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/unet.py` & `batchflow-0.8.1a0/batchflow/models/torch/unet.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/utils.py` & `batchflow-0.8.1a0/batchflow/models/torch/utils.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/torch/vgg.py` & `batchflow-0.8.1a0/batchflow/models/torch/vgg.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/models/utils.py` & `batchflow-0.8.1a0/batchflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/monitor.py` & `batchflow-0.8.1a0/batchflow/monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     pass
 try:
     import nvidia_smi
 except ImportError:
     # Use this value to raise ImportError later
     nvidia_smi = None
 
-from .plotter import plot
 from .decorators import deprecated
 
 
 
 class ResourceMonitor:
     """ Periodically runs supplied function in a separate thread and stores its outputs.
 
@@ -58,15 +57,15 @@
             self.ticks.append(time.time())
             time.sleep(self.frequency)
 
     def start(self):
         """ Start a separate thread with `function` calls every `frequency` seconds. """
         if not self.running:
             self.running = True
-            self.thread = Thread(target=self.endless_repeat)
+            self.thread = Thread(target=self.endless_repeat, name=f'BatchFlow-{type(self).__name__}')
             self.thread.start()
 
     def stop(self):
         """ Stop separate thread.
         Add another data point and timestamp to the containers, so that monitor has at least two measurements.
         """
         if self.running:
@@ -119,14 +118,15 @@
             'ylabel_rotation': 'horizontal',
             'ylabel_labelpad': 15,
             'grid': 'major',
             **kwargs
         }
 
         if plotter is None:
+            from .plotter import plot
             plotter = plot([None], mode='curve', combine='separate', ratio=1, scale=0.5)
 
         plot_config = {**plotter.config, **plot_config}
         return plotter(data=data, mode='curve', positions=positions, **plot_config)
 
     deprecation_msg = "`{}` is deprecated and will be removed in future versions, use `{}` instead."
     visualize = deprecated(deprecation_msg.format('ResourceMonitor.visualize', 'ResourceMonitor.plot'))(plot)
@@ -180,14 +180,44 @@
 
     @staticmethod
     def get_usage(process=None, **kwargs):
         """ Track current process virtual memory usage. """
         _ = kwargs
         return process.memory_info().vms / (1024 ** 3) # gbytes
 
+class SHRMonitor(ProcessResourceMonitor):
+    """ Track current process memory, potentially shared with other processes. """
+    UNIT = 'Gb'
+
+    @staticmethod
+    def get_usage(process=None, **kwargs):
+        """ Track current process unique virtual memory usage. """
+        _ = kwargs
+        return process.memory_info().shared / (1024 ** 3) # gbytes
+
+class CodeMonitor(ProcessResourceMonitor):
+    """ Track current process memory, devoted to executable code. """
+    UNIT = 'Gb'
+
+    @staticmethod
+    def get_usage(process=None, **kwargs):
+        """ Track current process unique virtual memory usage. """
+        _ = kwargs
+        return process.memory_info().text / (1024 ** 3) # gbytes
+
+class DataMonitor(ProcessResourceMonitor):
+    """ Track current process memory, devoted to anything but executable code. """
+    UNIT = 'Gb'
+
+    @staticmethod
+    def get_usage(process=None, **kwargs):
+        """ Track current process unique virtual memory usage. """
+        _ = kwargs
+        return process.memory_info().data / (1024 ** 3) # gbytes
+
 class USSMonitor(ProcessResourceMonitor):
     """ Track current process unique virtual memory usage. """
     UNIT = 'Gb'
 
     @staticmethod
     def get_usage(process=None, **kwargs):
         """ Track current process unique virtual memory usage. """
@@ -209,14 +239,18 @@
             env_variable = literal_eval(env_variable)
             gpu_list = list(env_variable) if isinstance(env_variable, tuple) else [env_variable]
 
         nvidia_smi.nvmlInit()
         gpu_handles = [nvidia_smi.nvmlDeviceGetHandleByIndex(i) for i in gpu_list]
         self.kwargs.update({'gpu_list': gpu_list, 'gpu_handles': gpu_handles})
 
+    def __del__(self):
+        super().__del__()
+        nvidia_smi.nvmlShutdown()
+
 
 class GPUMonitor(GPUResourceMonitor):
     """ Track GPU usage. """
     UNIT = '%'
 
     @staticmethod
     def get_usage(gpu_handles=None, **kwargs):
@@ -249,14 +283,17 @@
 
 
 MONITOR_ALIASES = {
     MemoryMonitor: ['mmonitor', 'memory', 'memorymonitor'],
     CPUMonitor: ['cmonitor', 'cpu', 'cpumonitor'],
     RSSMonitor: ['rss'],
     VMSMonitor: ['vms'],
+    SHRMonitor: ['shr', 'shared'],
+    CodeMonitor: ['code', 'text'],
+    DataMonitor: ['data'],
     USSMonitor: ['uss'],
     GPUMonitor: ['gpu'],
     GPUMemoryMonitor: ['gpu_memory'],
     GPUMemoryUtilizationMonitor: ['gpu_memory_utilization']
 }
 
 MONITOR_ALIASES = {alias: monitor for monitor, aliases in MONITOR_ALIASES.items()
@@ -282,21 +319,22 @@
     def __exit__(self, exc_type, exc_value, exc_traceback):
         for monitor in self:
             monitor.stop()
 
     def plot(self, plotter=None, positions=None, savepath=None, **kwargs):
         """ Visualize multiple monitors in a single figure. """
         plot_config = {
-            'ratio': 1 / len(self),
+            'ratio': 1 / min(len(self), 4),
             'scale': 0.5,
-            'ncols': None if 'nrows' in kwargs else len(self),
+            'ncols': None if 'nrows' in kwargs else min(len(self), 4),
             **kwargs
         }
 
         if plotter is None:
+            from .plotter import plot
             plotter = plot(data=[None] * len(self), mode='curve', combine='separate', **plot_config)
 
         positions = range(len(self))
         for position, monitor in zip(positions, self):
             monitor.plot(plotter=plotter, positions=position, **kwargs)
 
         if savepath is not None:
```

### Comparing `batchflow-0.8.1/batchflow/named_expr.py` & `batchflow-0.8.1a0/batchflow/named_expr.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/notifier.py` & `batchflow-0.8.1a0/batchflow/notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     from IPython import display
 except ImportError:
     pass
 
 from .named_expr import NamedExpression, eval_expr
 from .monitor import ResourceMonitor, MONITOR_ALIASES
 from .utils_telegram import TelegramMessage
-from .plotter import plot
-from .plotter.utils import PlotConfig
+
 
 
 
 class DummyBar:
     """ Progress tracker without visual representation. """
     #pylint: disable=invalid-name
     def __init__(self, total, *args, **kwargs):
@@ -234,14 +233,15 @@
                 'file': sys.stdout,
                 **kwargs
             }
 
         # Function to initialize / reinitialize bar, when needed
         if disable:
             bar_func = DummyBar
+            self.bar = None
             self.disable()
 
         self.bar = None
         self.bar_func = lambda total: bar_func(total=total, **kwargs)
 
         # Make bar with known / unknown total length
         self.total = None
@@ -274,15 +274,16 @@
         self.total = total
 
     def make_bar(self):
         """ Create new bar. Force close the previous, if needed. """
         if self.bar is not None:
             try:
                 # jupyter bar must be closed and reopened
-                self.bar.display(close=True)
+                if not getattr(self.bar, 'disable', False):
+                    self.bar.display(close=True)
                 self.bar = self.bar_func(total=self.total)
             except TypeError:
                 # text bar can work with a simple reassigning of `total`
                 self.bar.total = self.total
         else:
             self.bar = self.bar_func(total=self.total)
 
@@ -369,20 +370,21 @@
                 raise TypeError(f'Unknown type of `source`, {type(source)}!')
 
 
     def update_postfix(self):
         """ Set the new bar description, if needed. """
         postfix = self.create_description(iteration=-1)
 
-        previous_postfix = self.bar.postfix or ''
+        previous_postfix = getattr(self.bar, 'postfix', None) or ''
         if postfix and not previous_postfix.startswith(postfix):
             self.bar.set_postfix_str(postfix)
 
     def make_plotter(self, num_graphs=None, layout='horizontal', figsize=None, ncols=None, nrows=None, **kwargs):
         """ Make canvas for plotting graphs. """
+        from .plotter import plot
         if num_graphs is None:
             num_graphs = len(self.data_containers)
 
         if ncols is None and nrows is None:
             if layout in ['h', 'horizontal']:
                 ncols, nrows = num_graphs, 1
             elif layout in ['v', 'vertical']:
@@ -408,14 +410,15 @@
         }
 
         return plot(show=False, fix_config=True, **plot_config)
 
     def update_plot(self, index=0, add_suptitle=False, savepath=None, clear_display=True, show=True,
                     telegram=None, **kwargs):
         """ Draw plots anew. """
+        from .plotter.utils import PlotConfig
         plot_config = PlotConfig(kwargs)
 
         if clear_display:
             display.clear_output(wait=True)
 
         if add_suptitle:
             fmt = {
@@ -453,16 +456,20 @@
 
         data = container['data']
         source = container['source']
         name = container['name']
         plot_function = container.get('plot_function')
         plot_config = container.get('plot_config', {})
         plot_config = {**plot_config, **kwargs}
-        x = np.arange(len(data))[self.slice]
-        y = np.array(data)[self.slice]
+
+        x = np.arange(len(data))
+        y = data
+        if self.slice not in [None, slice(None)]:
+            x = np.array(x)[self.slice]
+            y = np.array(y)[self.slice]
 
         if plot_function is not None:
             plot_function(ax=subplot.ax, index=index, x=x, y=y, container=container, notifier=self, **plot_config)
         elif isinstance(source, ResourceMonitor):
             source.plot(plotter=self.plotter, positions=index, **plot_config)
         else:
             source_defaults = {'title': name}
```

### Comparing `batchflow-0.8.1/batchflow/once_pipeline.py` & `batchflow-0.8.1a0/batchflow/once_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/opensets/base.py` & `batchflow-0.8.1a0/batchflow/opensets/base.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/opensets/cifar.py` & `batchflow-0.8.1a0/batchflow/opensets/cifar.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/opensets/coco.py` & `batchflow-0.8.1a0/batchflow/opensets/coco.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/opensets/imagenette.py` & `batchflow-0.8.1a0/batchflow/opensets/imagenette.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/opensets/mnist.py` & `batchflow-0.8.1a0/batchflow/opensets/mnist.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/opensets/pascal.py` & `batchflow-0.8.1a0/batchflow/opensets/pascal.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/pipeline.py` & `batchflow-0.8.1a0/batchflow/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import time
 from functools import partial
 import threading
 import asyncio
 import logging
 import warnings
+from time import perf_counter
 
 from .base import Baseset
 from .config import Config
 from .batch import Batch
 from .decorators import deprecated
 from .exceptions import StopPipeline
 from .named_expr import NamedExpression, V, eval_expr
@@ -98,21 +99,23 @@
         self._rest_batch = None
         self.variables_initialised = False
         self._local = threading.local()
         self.random = None
         self.random_seed = None
 
         self._profiler = None
+        self.run_time = None
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state['random'] = getattr(self._local, 'random', None)
         state.pop('_local')
         state['_profiler'] = None
         state['_batch_generator'] = None
+        state['iter_params'] = None
         return state
 
     def __setstate__(self, state):
         self._local = threading.local()
         for k, v in state.items():
             setattr(self, k, v)
 
@@ -908,15 +911,16 @@
                     action['args'] = join_batches + action['args']
                     join_batches = None
 
                 batch, action_time = self._exec_one_action(batch, action, iteration=iteration)
 
             if self._profiler:
                 name = self.get_action_name(action, add_index=True)
-                self._profiler.disable(batch.iteration, name, batch_id=id(batch), action_time=action_time)
+                self._profiler.disable(iteration=batch.iteration, name=name,
+                                       batch_id=id(batch), action_time=action_time)
 
         return batch
 
     def show_profile_info(self, **kwargs):
         return self._profiler.show_profile_info(**kwargs)
 
     @property
@@ -1441,19 +1445,20 @@
             self.variables_initialised = True
 
         if 'models' in what:
             self.models.reset()
 
         self.random_seed = seed
 
-        if profile == 2 or isinstance(profile, str) and 'detailed'.startswith(profile):
-            self._profiler = PipelineProfiler(detailed=True)
-        elif profile == 1 or profile is True:
-            self._profiler = PipelineProfiler(detailed=False)
-        else: # 0, False, None
+        if self._profiler is None:
+            if profile == 2 or isinstance(profile, str) and 'detailed'.startswith(profile):
+                self._profiler = PipelineProfiler(detailed=True)
+            elif profile in [1, True]:
+                self._profiler = PipelineProfiler(detailed=False)
+        if profile in [0, False, None]:
             self._profiler = None
 
 
     def gen_rebatch(self, *args, **kwargs):
         """ Generate batches for rebatch operation """
         _action = self._actions[0]
 
@@ -1632,29 +1637,32 @@
     def run(self, *args, **kwargs):
         """ Execute all lazy actions for each batch in the dataset
 
         See also
         --------
         :meth:`~.Pipeline.gen_batch`
         """
+        start_time = perf_counter()
         if kwargs.pop('lazy', False):
             # if lazy is passed, then store params for later execution
             self._lazy_run = args, kwargs
             return self
 
         if len(args) == 0 and len(kwargs) == 0 and self._lazy_run is not None:
             args, kwargs = self._lazy_run
 
         args_value, kwargs_value = self._eval_run_args(args, kwargs)
 
         if kwargs_value.get('n_epochs', None) is None and kwargs_value.get('n_iters', None) is None:
             warnings.warn('Batch generation will never stop as ' \
                           'n_epochs=None and n_iters=None', RuntimeWarning)
 
-        return PipelineExecutor(self).run(*args_value, **kwargs_value)
+        PipelineExecutor(self).run(*args_value, **kwargs_value)
+        self.run_time = perf_counter() - start_time
+        return self
 
     def run_now(self, *args, **kwargs):
         """ Execute pipeline immediately """
         return self.run(*args, **kwargs, lazy=False)
 
     def run_later(self, *args, **kwargs):
         """ Define params to execute pipeline later """
```

### Comparing `batchflow-0.8.1/batchflow/pipeline_executor.py` & `batchflow-0.8.1a0/batchflow/pipeline_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
                 if ignore_exceptions:
                     batch = None
                 else:
                     batch = END_PIPELINE_SIGNAL
             finally:
                 self._prefetch_queue.task_done()
                 self._batch_queue.put(batch, block=True)
+                if batch == END_PIPELINE_SIGNAL:
+                    self._stop_flag = True
 
 
     def gen_batch(self, *args, dataset=None, rebatch=False, reset='iter', profile=False,
                   ignore_exceptions=False, **kwargs):
         """ Generate batches (see :meth:`~.Pipeline.gen_batch`) """
 
 
@@ -164,15 +166,16 @@
 
         if self.pipeline.before:
             self.pipeline.before.run()
 
         if prefetch > 0:
 
             if target in ['threads', 't']:
-                self._executor = cf.ThreadPoolExecutor(max_workers=prefetch + 1)
+                self._executor = cf.ThreadPoolExecutor(max_workers=prefetch + 1,
+                                                       thread_name_prefix='BatchFlow-PipelineExecutor')
             elif target in ['mpc', 'm']:
                 self._executor = cf.ProcessPoolExecutor(max_workers=prefetch + 1)
             else:
                 raise ValueError("target should be one of ['threads', 'mpc']")
 
             self._stop_flag = False
             # count queue warrants that exactly prefetch+1 num batches will be submitted to executor
@@ -182,35 +185,37 @@
             # most of the time exactly prefetch+1 items will be in the queue
             self._prefetch_queue = q.Queue()
             # batch queue holds batches ready to be yielded
             self._batch_queue = q.Queue()
             # due to count queue both prefetch and batch queue cannot contain more than prefetch+1 items
 
             # service executor runs batch generation and batch processing threads
-            self._service_executor = cf.ThreadPoolExecutor(max_workers=2)
+            self._service_executor = cf.ThreadPoolExecutor(max_workers=2,
+                                                           thread_name_prefix='BatchFlow-PipelineServiceExecutor')
             # this thread submits batches (waits for count queue and puts into prefetch queue)
             self._service_executor.submit(self._put_batches_into_queue, batch_generator, seed=execution_seed)
             # this thread gets processed batches (waits for futures to be complete and puts into batch queue)
             self._service_executor.submit(self._run_batches_from_queue, ignore_exceptions)
 
             # main thread gets ready batches and yield them one by one (releasing count queue after each one)
             while not self._stop_flag:
                 batch_res = self._batch_queue.get(block=True)
                 self._batch_queue.task_done()
-                if batch_res == END_PIPELINE_SIGNAL:
-                    self._stop_flag = True
-                else:
+                if batch_res != END_PIPELINE_SIGNAL:
                     # the batch has been created in another thread, so we need to set pipeline
                     if batch_res is not None:
                         batch_res.pipeline = self.pipeline
                     notifier.update(pipeline=self.pipeline, batch=batch_res)
                     yield batch_res
                     self._prefetch_count.get(block=True)
                     self._prefetch_count.task_done()
 
+            self._executor.shutdown()
+            self._service_executor.shutdown()
+
         else:
             # save RNG
             random = self.pipeline.random
 
             is_empty = True
             iteration = 1
             for batch in batch_generator:
```

### Comparing `batchflow-0.8.1/batchflow/plotter/plot.py` & `batchflow-0.8.1a0/batchflow/plotter/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
             data = np.ma.array(data, mask=mask)
         return data
 
     def smooth(self, data):
         """ Calculate running average on given data with provided window. """
         window = self.config.get('window')
         if window is not None and window < len(data):
+            data = np.array(data, dtype='float32')
             data = convolve(data, np.ones(window), mode='nearest') / window
             return data
         return None
 
     def preprocess(self, data):
         """ Look through layer config for requested data transformations and apply them. """
         if self.mode == 'image':
@@ -1594,14 +1595,15 @@
         save_keys = ['savepath', 'bbox_inches', 'pad_inches', 'dpi']
         save_config = self.config.filter(keys=save_keys, prefix='save_')
         save_config.update(kwargs)
 
         default_savepath = datetime.now().strftime('%Y-%m-%d_%H:%M:%S.png')
         savepath = save_config.pop('savepath', default_savepath)
 
-        self.figure.savefig(fname=savepath, **save_config)
+        if savepath:
+            self.figure.savefig(fname=savepath, **save_config)
 
     def close(self):
         """ Close figure. """
         plt.close(self.figure)
 
 plot = Plot # an alias
```

### Comparing `batchflow-0.8.1/batchflow/plotter/utils.py` & `batchflow-0.8.1a0/batchflow/plotter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from colorsys import rgb_to_hls, hls_to_rgb
 from numbers import Number
 import operator
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from matplotlib.collections import PatchCollection
-from matplotlib.colors import ColorConverter, ListedColormap, to_rgba
-from matplotlib.patches import Rectangle
-from matplotlib.legend_handler import HandlerBase
+try:
+    from matplotlib.collections import PatchCollection
+    from matplotlib.colors import ColorConverter, ListedColormap, to_rgba
+    from matplotlib.patches import Rectangle
+    from matplotlib.legend_handler import HandlerBase
+except ImportError:
+    pass
 
 try:
     from numba import njit
 except ImportError:
     from ..decorators import njit
 
 class CycledList(list):
```

### Comparing `batchflow-0.8.1/batchflow/profiler.py` & `batchflow-0.8.1a0/batchflow/profiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,112 @@
 """ Profiler for batchflow units """
-
-import time
+from time import perf_counter
 from pstats import Stats
 from cProfile import Profile
 import threading
 import warnings
 
 try:
     import pandas as pd
 except ImportError:
     from . import _fake as pd
 
+
+
 class Profiler:
     """ Profiler for batchflow units.
 
     Parameters
     ----------
     profile : bool or {0, 1, 2} or 'detailed'
         whether to use profiler
     """
-
     UNIT_NAME = 'action'
 
+
     def __init__(self, detailed=True):
-        if detailed:
-            self.detailed = True
-            self._profiler = Profile()
-        else:
-            self.detailed = False
-            self._profiler = None
+        self.start_time = None
+        self.detailed = detailed
+        self.profiler = Profile() if detailed else None
+        self.iteration = 0
 
-        self._profile_info = []
+        self._profile_info = []  # list of dicts with info about each item
         self._profile_info_lock = threading.Lock()
-        self.start_time = None
 
     @property
     def profile_info(self):
-        return pd.concat(self._profile_info)
+        """ Prepare profile results dataframe. """
+        if not self._profile_info:
+            return None
+        df = pd.DataFrame(self._profile_info).set_index('name').sort_values('iter')
+        df.index.name = self.UNIT_NAME
+
+        n_unique_units = df.index.unique().size
+        df['iter'] = df['iter'] // n_unique_units + 1
+        return df
 
     def enable(self):
-        """ Enable profiling. """
-        self.start_time = time.time()
+        """ Start profiling. """
+        self.start_time = perf_counter()
         if self.detailed:
-            self._profiler.enable()
+            self.profiler.enable()
 
     def disable(self, iteration, name, **kwargs):
         """ Disable profiling. """
-        if self.detailed:
-            self._profiler.disable()
-        total_time = time.time() - self.start_time
-        self._add_profile_info(iteration, name, start_time=self.start_time, total_time=total_time, **kwargs)
+        total_time = perf_counter() - self.start_time
 
-    def _add_profile_info(self, iter_no, name, total_time, **kwargs):
         if self.detailed:
-            stats = Stats(self._profiler)
-            self._profiler.clear()
+            self.profiler.disable()
+            stats = Stats(self.profiler)
+            self.profiler.clear()
 
-            indices, values = [], []
+            values = []
             for key, value in stats.stats.items():
                 for k, v in value[4].items():
-                    # action name, method_name, file_name, line_no, callee
-                    indices.append((name, '{}::{}::{}::{}'.format(key[2], *k)))
+                    call_id = f'{key[2]}::{k[0]}::{k[1]}::{k[2]}' # method_name, file_name, line_no, callee
                     row_dict = {
-                        'iter': iter_no, 'total_time': total_time, 'eval_time': stats.total_tt, # base stats
+                        'name': name, 'id': call_id,
+                        'iter': self.iteration, 'outer_iter': iteration,
+                        'total_time': total_time, 'eval_time': stats.total_tt, # base stats
                         'ncalls': v[0], 'tottime': v[2], 'cumtime': v[3], # detailed stats
                         **kwargs
                     }
                     values.append(row_dict)
         else:
-            indices = [(name, '')]
-            values = [{'iter': iter_no, 'total_time': total_time, 'eval_time': total_time,
-                    **kwargs}]
-
-        multiindex = pd.MultiIndex.from_tuples(indices, names=[self.UNIT_NAME, 'id'])
-        df = pd.DataFrame(values, index=multiindex)
+            values = [{
+                'name': name,
+                'iter': self.iteration, 'outer_iter': iteration,
+                'total_time': total_time,
+                **kwargs
+            }]
 
         with self._profile_info_lock:
-            self._profile_info.append(df)
+            self._profile_info.extend(values)
+            self.iteration += 1
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state.pop('_profile_info_lock')
-        state['_profiler'] = None
+        state['profiler'] = None
         return state
 
     def __setstate__(self, state):
-        self._profile_info_lock = threading.Lock()
         for k, v in state.items():
             setattr(self, k, v)
 
+        self.profiler = Profiler() if self.detailed else None
+        self._profile_info_lock = threading.Lock()
+
+    def __add__(self, other):
+        """ Combine multiple profilers with their collected info concatenated. """
+        new = type(self)(detailed=self.detailed)
+        new._profile_info = self._profile_info + other._profile_info
+        return new
+
+
 class PipelineProfiler(Profiler):
     """ Profiler for batchflow pipelines. """
     def show_profile_info(self, per_iter=False, detailed=False,
                           groupby=None, columns=None, sortby=None, limit=10):
         """ Show stored profiling information with varying levels of details.
 
         Parameters
@@ -109,43 +123,45 @@
             Column id to sort on. Note that if data is aggregated over iters (`per_iter` is False),
             then it must be a full identificator of a column.
         limit : int
             Limits the length of resulting dataframe.
         parse : bool
             Allows to re-create underlying dataframe from scratches.
         """
-        if self.profile_info is None:
+        profile_info = self.profile_info
+        if profile_info is None:
             warnings.warn("Profiling has not been enabled.")
             return None
 
         detailed = False if not self.detailed else detailed
 
         if per_iter is False and detailed is False:
-            columns = columns or ['total_time', 'eval_time']
+            columns = columns or ['total_time']
             sortby = sortby or ('total_time', 'sum')
             aggs = {key: ['sum', 'mean', 'max'] for key in columns}
-            result = (self.profile_info.groupby(['action', 'iter'])[columns].mean().groupby('action').agg(aggs)
+            result = (profile_info.groupby(['action', 'iter'])[columns]
+                      .mean(numeric_only=True).groupby('action').agg(aggs, numeric_only=True)
                       .sort_values(sortby, ascending=False))
 
         elif per_iter is False and detailed is True:
             columns = columns or ['ncalls', 'tottime', 'cumtime']
             sortby = sortby or ('tottime', 'sum')
             aggs = {key: ['sum', 'mean', 'max'] for key in columns}
-            result = (self.profile_info.reset_index().groupby(['action', 'id']).agg(aggs)
+            result = (profile_info.reset_index().groupby(['action', 'id']).agg(aggs, numeric_only=True)
                       .sort_values(['action', sortby], ascending=[True, False])
                       .groupby(level=0).apply(lambda df: df[:limit]).droplevel(0))
 
         elif per_iter is True and detailed is False:
             groupby = groupby or ['iter', 'action']
-            columns = columns or ['action', 'total_time', 'eval_time', 'batch_id']
+            columns = columns or ['action', 'total_time', 'batch_id']
             sortby = sortby or 'total_time'
-            result = (self.profile_info.reset_index().groupby(groupby)[columns].mean()
+            result = (profile_info.reset_index().groupby(groupby)[columns].mean(numeric_only=True)
                       .sort_values(['iter', sortby], ascending=[True, False]))
 
         elif per_iter is True and detailed is True:
             groupby = groupby or ['iter', 'action', 'id']
             columns = columns or ['ncalls', 'tottime', 'cumtime']
             sortby = sortby or 'tottime'
-            result = (self.profile_info.reset_index().set_index(groupby)[columns]
+            result = (profile_info.reset_index().set_index(groupby)[columns]
                       .sort_values(['iter', 'action', sortby], ascending=[True, True, False])
                       .groupby(level=[0, 1]).apply(lambda df: df[:limit]).droplevel([0, 1]))
         return result
```

### Comparing `batchflow-0.8.1/batchflow/research/distributor.py` & `batchflow-0.8.1a0/batchflow/research/distributor.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/research/domain.py` & `batchflow-0.8.1a0/batchflow/research/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         self.n_reps = 1
         self.repeat_each = None
         self.n_updates = 0
         self.additional = True
         self.create_id_prefix = False
         self.random_state = None
 
-        self.values_indices = dict()
+        self.values_indices = {}
 
     def _get_all_options_names(self):
         options = []
         for cube in self.cubes:
             for option in cube:
                 alias = option[0].alias
                 if alias not in options and alias != 'repetition':
@@ -321,15 +321,15 @@
         self.random_state = make_rng(seed)
         self.reset_iter()
 
     def set_update(self, function, when, **kwargs):
         """ Set domain update parameters. """
         if isinstance(when, (int, str)):
             when = [when]
-        iter_kwargs = dict()
+        iter_kwargs = {}
         for attr in ['n_items', 'n_reps', 'repeat_each']:
             iter_kwargs[attr] = kwargs.pop(attr) if attr in kwargs else getattr(self, attr)
         self.updates.append({
             'function': function,
             'when': when,
             'kwargs': kwargs,
             'iter_kwargs': iter_kwargs
@@ -588,15 +588,15 @@
         """
         if not isinstance(values, (list, tuple, np.ndarray)):
             raise TypeError(f'`values` must be array-like object but {type(values)} were given')
         res = []
         for value in values:
             if self.create_id_prefix:
                 n_digits = self.create_id_prefix if self.create_id_prefix is not True else 1
-                option_values = self.values_indices.get(name.alias, dict())
+                option_values = self.values_indices.get(name.alias, {})
                 current_index = option_values.get(value.alias, len(option_values))
                 option_values[value.alias] = current_index
                 self.values_indices[name.alias] = option_values
                 fmt = ("{:0" + str(n_digits) + "d}").format(current_index)
                 res.append(ConfigAlias([[name, value], ["#" + name.alias, fmt]]))
             else:
                 res.append(ConfigAlias([[name, value]]))
```

### Comparing `batchflow-0.8.1/batchflow/research/experiment.py` & `batchflow-0.8.1a0/batchflow/research/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,15 @@
 
 
         self._is_alive = True # should experiment be executed or not. Becomes False when Exceptions was raised and all
                               # units for these iterations were executed.
         self._is_failed = False # was an exception raised or not
 
         self.last = False
-        self.outputs = dict()
+        self.outputs = {}
         self.storage = None
         self.has_dump = False # does unit has any dump actions or not
         self.name = None # name of the executor/research
         self.dump_results = None
         self.loglevel = None
         self.monitor = None
         self.id = None #pylint:disable=invalid-name
@@ -831,15 +831,15 @@
                 self.n_branches = len(branches_configs)
         else:
             if branches_configs is not None and len(configs) != len(branches_configs):
                 raise ValueError('`configs` and `branches_configs` must be of the same length.')
             self.n_branches = len(configs)
 
         self.configs = configs or [Config() for _ in range(self.n_branches)]
-        self.executor_config = Config(executor_config or dict())
+        self.executor_config = Config(executor_config or {})
         self.branches_configs = branches_configs or [Config() for _ in range(self.n_branches)]
         self.branches_configs = [Config(config) for config in self.branches_configs]
         self.n_iters = n_iters
         self.research = research
         self.experiment_template = experiment
         self.task_name = task_name or 'Task'
         self.target = target
@@ -875,19 +875,19 @@
             'debug': False,
             'profile': False,
             'redirect_stdout': True,
             'redirect_stderr': True,
             'dump_results': False,
             'finalize': False
         }
-        for attr in defaults:
+        for attr, value_ in defaults.items():
             if self.research:
                 value = getattr(self.research, attr)
             else:
-                value = kwargs.get(attr, defaults[attr])
+                value = kwargs.get(attr, value_)
             setattr(self, attr, value)
 
     def create_experiments(self):
         """ Initialize experiments. """
         self.experiments = []
         for index, (config, branch_config) in enumerate(zip(self.configs, self.branches_configs)):
             full_config = ConfigAlias(config) + ConfigAlias(branch_config) + ConfigAlias(self.executor_config)
@@ -911,15 +911,15 @@
 
             for iteration in iterations:
                 for unit_name, unit in self.experiment_template.actions.items():
                     if unit.root or len(self.experiments) == 1:
                         self.call_root(iteration, unit_name)
                     else:
                         self.parallel_call(iteration, unit_name, target=self.target, debug=self.debug) #pylint:disable=unexpected-keyword-arg
-                if not any([experiment.is_alive for experiment in self.experiments]):
+                if not any(experiment.is_alive for experiment in self.experiments):
                     break
                 if self.research:
                     for experiment in self.experiments:
                         if experiment.is_alive:
                             self.research.monitor.execute_iteration(experiment)
 
             for index, experiment in enumerate(self.experiments):
```

### Comparing `batchflow-0.8.1/batchflow/research/named_expr.py` & `batchflow-0.8.1a0/batchflow/research/named_expr.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/research/profiler.py` & `batchflow-0.8.1a0/batchflow/research/profiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 try:
     import pandas as pd
 except ImportError:
     from . import _fake as pd
 
 from ..profiler import Profiler
 
+
 class ExperimentProfiler(Profiler):
     """ Profiler for Research experiments. """
 
     UNIT_NAME = 'unit'
 
     def show_profile_info(self, per_iter=False, per_experiment=False, detailed=False,
                           groupby=None, columns=None, sortby=None, limit=10):
@@ -44,41 +45,41 @@
             warnings.warn("Profiling has not been enabled.")
             return None
 
         detailed = False if not self.detailed else detailed
 
         if per_iter is False and detailed is False:
             groupby = ['experiment', 'unit', 'iter'] if per_experiment else ['unit', 'iter']
-            columns = columns or ['total_time', 'eval_time', 'unit_time']
+            columns = columns or ['total_time', 'unit_time']
             sortby = sortby or ('total_time', 'sum')
             aggs = {key: ['sum', 'mean', 'max'] for key in columns}
-            result = (self.profile_info.groupby(groupby)[columns].mean()
-                      .groupby(groupby[:-1]).agg(aggs)
+            result = (self.profile_info.groupby(groupby)[columns].mean(numeric_only=True)
+                      .groupby(groupby[:-1]).agg(aggs, numeric_only=True)
                       .sort_values(sortby, ascending=False))
 
             if per_experiment:
                 result = result.sort_index(level=0)
 
         elif per_iter is False and detailed is True:
             groupby = ['experiment', 'unit', 'id'] if per_experiment else ['unit', 'id']
             columns = columns or ['ncalls', 'tottime', 'cumtime']
             sortby = sortby or ('tottime', 'sum')
             aggs = {key: ['sum', 'mean', 'max'] for key in columns}
             level = [0, 1] if per_experiment else 0
-            result = (self.profile_info.reset_index().groupby(groupby).agg(aggs)
+            result = (self.profile_info.reset_index().groupby(groupby).agg(aggs, numeric_only=True)
                     .sort_values([*groupby[:-1], sortby], ascending=[True] * (len(groupby)-1) + [False])
                     .groupby(level=level).apply(lambda df: df.iloc[:limit].reset_index(level)))
 
         elif per_iter is True and detailed is False:
             groupby = groupby or ['iter', 'unit']
             groupby = ['experiment', *groupby] if per_experiment else groupby
 
-            columns = columns or ['unit', 'total_time', 'eval_time', 'unit_time']
+            columns = columns or ['unit', 'total_time', 'unit_time']
             sortby = sortby or 'total_time'
-            result = (self.profile_info.reset_index().groupby(groupby)[columns].mean()
+            result = (self.profile_info.reset_index().groupby(groupby)[columns].mean(numeric_only=True)
                       .sort_values([*groupby[:-1], sortby], ascending=[True] * (len(groupby)-1) + [False]))
 
         elif per_iter is True and detailed is True:
             groupby = groupby or ['iter', 'unit', 'id']
             groupby = ['experiment', *groupby] if per_experiment else groupby
 
             columns = columns or ['ncalls', 'tottime', 'cumtime']
```

### Comparing `batchflow-0.8.1/batchflow/research/research.py` & `batchflow-0.8.1a0/batchflow/research/research.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self.n_reps = n_reps
         self.repeat_each = repeat_each
         self.create_id_prefix = False
         self.redirect_stdout = True
         self.redirect_stderr = True
         self.storage = None
 
-        self._env = dict() # current state of git repo and other environment information.
+        self._env = {} # current state of git repo and other environment information.
 
         self.workers = 1
         self.branches = 1
         self.n_iters = None
         self.devices = None
         self.executor_class = Executor
         self.dump_results = True
@@ -447,17 +447,17 @@
                   'parallel', 'loglevel', 'executor_target', 'executor_class']
         params_repr = []
         for param in params:
             params_repr += [f"{param}: {getattr(self, param, None)}"]
         params_repr = '\n'.join(params_repr)
 
         items = {'params': params_repr, 'experiment': str(self.experiment), 'domain': str(self.domain)}
-        for name in items:
+        for name, items_ in items.items():
             repr += f"{name}:\n"
-            repr += '\n'.join([spacing + item for item in str(items[name]).split('\n')])
+            repr += '\n'.join([spacing + item for item in str(items_).split('\n')])
             repr += 2 * '\n'
 
         return repr
 
     @classmethod
     def load(cls, name):
         """ Load research. """
```

### Comparing `batchflow-0.8.1/batchflow/research/results.py` & `batchflow-0.8.1a0/batchflow/research/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """ Research results. """
 
 import os
 import functools
 from collections import OrderedDict
 import glob
+
 import multiprocess as mp
-import pandas as pd
+try:
+    import pandas as pd
+except ImportError:
+    pass
 import numpy as np
 
 from ..utils import to_list
 from .utils import deserialize
 
 class ResearchResults:
     """ Class to collect, load and process research results.
@@ -25,15 +29,15 @@
     """
     def __init__(self, name, dump_results=True, **kwargs):
         self.name = name
         self.dump_results = dump_results
         self._manager = mp.Manager()
         self.results = self._manager.dict()
         self.configs = self._manager.dict()
-        self.artifacts = dict()
+        self.artifacts = {}
         self.kwargs = kwargs
 
         if dump_results and os.path.exists(name):
             self.load()
 
     def put(self, experiment_id, results, config):
         self.results[experiment_id] = results
@@ -76,15 +80,15 @@
             the same as config but with aliased values, by default None.
         domain : Domain, optional
             domain with parameters values to load, by default None.
         kwargs : dict
             is used as `config`. If `config` is not defined but `alias` is, then will be concated to `alias`.
         """
         experiment_id, name, iterations = self.filter(experiment_id, name, iterations, config, alias, domain, **kwargs)
-        results = dict()
+        results = {}
         for path in glob.glob(os.path.join(self.name, 'experiments', '*', 'results', '*')):
             path = os.path.normpath(path)
             _experiment_id, _, _name = path.split(os.sep)[-3:]
             if experiment_id is None or _experiment_id in experiment_id:
                 if name is None or _name in name:
                     if _experiment_id not in results:
                         results[_experiment_id] = OrderedDict()
@@ -112,15 +116,15 @@
         alias : Config, optional
             the same as config but with aliased values, by default None
         domain : Domain, optional
             domain with parameters values to load, by default None
         kwargs : dict
             is used as `config`. If `config` is not defined but `alias` is, then will be concated to `alias`.
         """
-        self.artifacts = dict()
+        self.artifacts = {}
         names = to_list('*' if name is None else name)
         experiment_id, _, _ = self.filter(experiment_id, None, None, config, alias, domain, **kwargs)
         for _name in names:
             for path in glob.glob(os.path.join(self.name, 'experiments', '*', _name)):
                 if os.path.basename(path) not in ['results', 'config.dill', 'config.json', 'experiment.log']:
                     path = os.path.normpath(path)
                     _experiment_id, _name = path.split(os.sep)[-2:]
@@ -237,15 +241,15 @@
     def load_iteration_files(self, path, iterations):
         """ Load files for specified iterations from specified path. """
         filenames = glob.glob(os.path.join(path, '*'))
         if iterations is None:
             files_to_load = {int(os.path.basename(filename)): filename for filename in filenames}
         else:
             dumped_iteration = np.sort(np.array([int(os.path.basename(filename)) for filename in filenames]))
-            files_to_load = dict()
+            files_to_load = {}
             for iteration in iterations:
                 _it = dumped_iteration[np.argwhere(dumped_iteration >= iteration)[0, 0]]
                 files_to_load[_it] = os.path.join(path, str(_it))
         files_to_load = OrderedDict(sorted(files_to_load.items()))
         results = OrderedDict()
         for filename in files_to_load.values():
             with open(filename, 'rb') as f:
@@ -324,16 +328,15 @@
             dataframe with name of the id of the experiment, artifact full path (with path to research folder)
             and relative path (inner path in research folder). Also can include experiment config.
         """
         if self.dump_results:
             self.load_configs()
             self.load_artifacts(**kwargs)
             df = []
-            for experiment_id in self.artifacts:
-                artifacts = self.artifacts[experiment_id]
+            for experiment_id, artifacts in self.artifacts.items():
                 df += [pd.DataFrame({'id': [experiment_id], **artifact}) for artifact in artifacts]
             if len(df) > 0:
                 df = pd.concat(df)
                 if include_config:
                     df = pd.merge(self.configs_to_df(use_alias, concat_config, remove_auxilary, drop_columns),
                                 df, how='inner', on='id')
                 return df
```

### Comparing `batchflow-0.8.1/batchflow/research/storage.py` & `batchflow-0.8.1a0/batchflow/research/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         path = os.path.join(name, 'experiments', self.experiment.id, 'experiment.log')
         self.logger = create_logger(logger_name, path, self.loglevel)
 
     def _dump_config(self):
         """ Dump config as serialized ConfigAlias instance and as a dict in JSON. """
         with open(os.path.join(self.full_path, 'config.dill'), 'wb') as file:
             dill.dump(self.experiment.config_alias, file)
-        with open(os.path.join(self.full_path, 'config.json'), 'w') as file:
+        with open(os.path.join(self.full_path, 'config.json'), 'w', encoding='utf-8') as file:
             json.dump(jsonify(self.experiment.config_alias.alias().config), file)
 
     def create_redirection_streams(self):
         """ Create streams to redirect stdout and stderr (if needed). """
         self.stdout_file = create_output_stream(
             self.experiment.redirect_stdout, True, 'stdout.txt', path=self.full_path, common=False
         )
@@ -382,14 +382,15 @@
         for filename, command in all_commands:
             if command.startswith('#'):
                 if command[1:] == 'python':
                     result = sys.version
                 else:
                     raise ValueError(f'Unknown env: {command}')
             else:
+                #pylint: disable=consider-using-with
                 process = subprocess.Popen(command.split(), stdout=subprocess.PIPE, cwd=cwd)
                 output, _ = process.communicate()
                 result = output.decode('utf')
             if replace is not None:
                 for key, value in replace.items():
                     result = re.sub(key, value, result)
 
@@ -439,15 +440,15 @@
         self.results = ResearchResults(self.research.name, False)
         self.profiler = ResearchProfiler(self.research.name, self.research.profile)
 
         self._manager = mp.Manager()
         self.experiments_stdout = self._manager.dict()
         self.experiments_stderr = self._manager.dict()
 
-        self._env = dict()
+        self._env = {}
 
         self.experiment_storage_class = MemoryExperimentStorage
 
     def close(self):
         """ Close shared memory managers. """
         super().close()
         self.experiments_stdout = dict(self.experiments_stdout)
@@ -522,15 +523,15 @@
             path = os.path.join(self.path, subfolder)
             if not os.path.exists(path):
                 os.makedirs(path)
 
     def _dump_research(self, research):
         with open(os.path.join(self.path, 'research.dill'), 'wb') as f:
             dill.dump(research, f)
-        with open(os.path.join(self.path, 'research.txt'), 'w') as f:
+        with open(os.path.join(self.path, 'research.txt'), 'w', encoding='utf-8') as f:
             f.write(str(research))
 
     def _create_logger(self):
         path = os.path.join(self.research.name, 'research.log')
         self.logger = create_logger(self.research.name, path, self.loglevel)
 
     def create_redirection_streams(self):
@@ -542,25 +543,25 @@
             self.research.redirect_stderr, True, 'stderr.txt', self.research.name, common=True
         )
 
     def _store_env(self, result, dst, filename):
         subfolder = os.path.join(self.path, 'env', dst)
         if not os.path.exists(subfolder):
             os.makedirs(subfolder)
-        with open(os.path.join(subfolder, filename + '.txt'), 'a') as file:
+        with open(os.path.join(subfolder, filename + '.txt'), 'a', encoding='utf-8') as file:
             file.write(result)
 
     @property
     def env(self):
         """ Environment state. """
-        env = dict()
+        env = {}
         filenames = glob.glob(os.path.join(self.path, 'env', '*'))
         for filename in filenames:
             name = os.path.splitext(os.path.basename(filename))[0]
-            with open(filename, 'r') as file:
+            with open(filename, 'r', encoding='utf-8') as file:
                 env[name] = file.read().strip()
         return env
 
     @classmethod
     def remove(cls, name, ask=True, force=False):
         """ Remove research folder.
```

### Comparing `batchflow-0.8.1/batchflow/research/utils.py` & `batchflow-0.8.1a0/batchflow/research/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 import os
 import logging
 import hashlib
 import io
 import contextlib
 import warnings
 from copy import deepcopy
+
 import dill
 import numpy as np
-import pandas as pd
+try:
+    import pandas as pd
+except ImportError:
+    pass
 
 from ..plotter import plot
 from ..plotter.plot import Subplot
 from ..utils import to_list
 
 
 class MultiOut:
@@ -133,24 +137,25 @@
     name = config.alias()['_prefix'] if create_prefix else ''
     name += hashlib.md5(config.alias(as_string=True).encode('utf-8')).hexdigest()[:8]
     name += ''.join(str(i) for i in random.integers(10, size=8))
     return name
 
 def create_output_stream(redirect, dump=False, filename=None, path=None, common=True):
     """ Create stream to redirect stdout/stderr. """
+    #pylint: disable=consider-using-with
     if bool(redirect):
         values = [1, 3] if common else [2, 3]
         if redirect in values:
             if dump:
                 filename = os.path.join(path, filename)
-                file = open(filename, 'a')
+                file = open(filename, 'a', encoding='utf-8')
             else:
                 file = io.StringIO()
         else:
-            file = open(os.devnull, 'w')
+            file = open(os.devnull, 'w', encoding='utf-8')
     else:
         file = contextlib.nullcontext()
     return file
 
 def plot_research(df, variables=None, subplots=None, aggregate=None, aggregate_fn='mean', same_color=None, layout=None,
                   short_label=True, ignore=('id', 'name'), meta=('id', 'config', 'repetition', 'cv_split'), **kwargs):
     """ Plot graphs of variables logged during research. Subplots are grouped by variables name by default.
```

### Comparing `batchflow-0.8.1/batchflow/run_notebook.py` & `batchflow-0.8.1a0/batchflow/run_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     """ Save notebook as ipynb file."""
     from nbconvert import HTMLExporter
     from IPython.display import display, FileLink
 
     html_exporter = HTMLExporter()
     body, _ = html_exporter.from_notebook_node(notebook)
 
-    with open(out_path_html, 'w') as f:
+    with open(out_path_html, 'w', encoding='utf-8') as f:
         f.write(body)
 
     if display_link:
         display(FileLink(out_path_html))
 
 
 def extract_traceback(notebook):
```

### Comparing `batchflow-0.8.1/batchflow/sampler.py` & `batchflow-0.8.1a0/batchflow/sampler.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/apply_parallel_test.py` & `batchflow-0.8.1a0/batchflow/tests/apply_parallel_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/assemble_test.py` & `batchflow-0.8.1a0/batchflow/tests/assemble_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/common_index_test.py` & `batchflow-0.8.1a0/batchflow/tests/common_index_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     path = 'fi_test_tmp'
 
     folders = [path]
 
     for folder in folders:
         os.mkdir(folder)
         for i in range(5):
-            open(os.path.join(folder, f'file_{i}.txt'), 'w').close()
+            with open(os.path.join(folder, f'file_{i}.txt'), 'w', encoding='utf-8'):
+                pass
 
     def fin():
         shutil.rmtree(path)
 
     request.addfinalizer(fin)
     return path, [name for name in os.listdir(path) if name.endswith('txt')]
```

### Comparing `batchflow-0.8.1/batchflow/tests/components_batch_test.py` & `batchflow-0.8.1a0/batchflow/tests/components_batch_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/components_test.py` & `batchflow-0.8.1a0/batchflow/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/config_basic_test.py` & `batchflow-0.8.1a0/batchflow/tests/config_basic_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/config_test.py` & `batchflow-0.8.1a0/batchflow/tests/config_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 sys.path.append('..')
 from batchflow import Config
 
 
 @pytest.fixture
 def config():
-    _config = dict(key1='val1', key2=dict())
+    _config = dict(key1='val1', key2={})
     _config['key2']['subkey1'] = 'val21'
     return Config(_config)
 
 
 class TestConfig:
     def test_getitem_key(self, config):
         assert config['key1'] == config.config['key1']
```

### Comparing `batchflow-0.8.1/batchflow/tests/conftest.py` & `batchflow-0.8.1a0/batchflow/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/dataset_test.py` & `batchflow-0.8.1a0/batchflow/tests/dataset_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/datasetindex_test.py` & `batchflow-0.8.1a0/batchflow/tests/datasetindex_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/filesindex_test.py` & `batchflow-0.8.1a0/batchflow/tests/filesindex_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     folder2 = 'other_folder'
 
     folders = [path, os.path.join(path, folder1), os.path.join(path, folder2)]
 
     for folder in folders:
         os.mkdir(folder)
         for i in range(3):
-            open(os.path.join(folder, f'file_{i}.txt'), 'w').close()
+            with open(os.path.join(folder, f'file_{i}.txt'), 'w', encoding='utf-8'):
+                pass
 
     def fin():
         shutil.rmtree(path)
 
     request.addfinalizer(fin)
     return path, folder1, folder2
```

### Comparing `batchflow-0.8.1/batchflow/tests/metrics_test.py` & `batchflow-0.8.1a0/batchflow/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/model_save_load_test.py` & `batchflow-0.8.1a0/batchflow/tests/model_save_load_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/named_expr_test.py` & `batchflow-0.8.1a0/batchflow/tests/named_expr_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/notebooks_test.py` & `batchflow-0.8.1a0/batchflow/tests/notebooks_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
 os.environ["CUDA_VISIBLE_DEVICES"] = "6"
 
 import warnings
 from glob import glob
 import pytest
-from tensorflow.test import is_gpu_available
+import torch
 
 
 
-NO_GPU = pytest.mark.skipif(not is_gpu_available(), reason='No GPU')
+NO_GPU = pytest.mark.skipif(not torch.cuda.is_available(), reason='No GPU')
 
 NOTEBOOKS_DIR = './notebooks/'
 NOTEBOOKS = glob(NOTEBOOKS_DIR + '*.ipynb')
 
 TUTORIALS_DIR = './../../examples/tutorials/'
 TUTORIALS = glob(TUTORIALS_DIR + '*.ipynb')
 ALLOWED_TUTORIALS = [
```

### Comparing `batchflow-0.8.1/batchflow/tests/plot_notebooks_test.py` & `batchflow-0.8.1a0/batchflow/tests/plot_notebooks_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/rebatch_test.py` & `batchflow-0.8.1a0/batchflow/tests/rebatch_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/regression_metrics_test.py` & `batchflow-0.8.1a0/batchflow/tests/regression_metrics_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/research_test.py` & `batchflow-0.8.1a0/batchflow/tests/research_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,15 +512,15 @@
         else:
             # id includes prefix for each parameter, repetition index and hash
             n_params = 2 if domain is not None else 0
             assert research.results.df.id.apply(lambda x: len(x.split('_')) == n_params + 2).all()
             parsed_id = research.results.df.id.apply(lambda x: x.split('_'))
 
             # check the number of digits for each prefix code
-            assert parsed_id.apply(lambda x: all([len(i) == create_id_prefix for i in x[:-1]])).all()
+            assert parsed_id.apply(lambda x: all(len(i) == create_id_prefix for i in x[:-1])).all()
 
 
     def test_remove(self, simple_research):
         simple_research.run(n_iters=1)
         assert os.path.exists(simple_research.name)
 
         Research.remove(simple_research.name, ask=False)
@@ -533,31 +533,31 @@
         def func():
             raise NotImplementedError
 
         with expectation:
             research = Research().add_callable(func)
             research.run(dump_results=False, executor_target='f', parallel=False, debug=debug)
 
-    @pytest.mark.parametrize('profile, shape', list(zip([2, 1], [9, 6])))
+    @pytest.mark.parametrize('profile, shape', list(zip([2, 1], [10, 5])))
     def test_profile(self, profile, shape, simple_research):
         simple_research.run(n_iters=3, dump_results=False, profile=profile)
 
         assert simple_research.profiler.profile_info.shape[1] == shape
 
     @pytest.mark.parametrize('loglevel, length_res, length_exp', list(zip(['info', 'debug'], [62, 104], [7, 14])))
     def test_logging(self, loglevel, length_res, length_exp, tmp_path, simple_research):
         path = os.path.join(tmp_path, 'research')
         simple_research.run(name=path, n_iters=3, dump_results=True, loglevel=loglevel)
 
-        with open(os.path.join(path, 'research.log')) as file:
+        with open(os.path.join(path, 'research.log'), encoding='utf-8') as file:
             lines = file.readlines()
             assert len(lines) == length_res
 
         for path in glob.glob(os.path.join(path, 'experiments', '*')):
-            with open(os.path.join(path, 'experiment.log')) as file:
+            with open(os.path.join(path, 'experiment.log'), encoding='utf-8') as file:
                 lines = file.readlines()
                 assert len(lines) == length_exp
 
     def test_coincided_names(self):
         def f(a):
             return a ** 10
 
@@ -606,23 +606,23 @@
                 if dump_results:
                     n_files = len(research.results.artifacts_to_df(name=filename))
                     assert (filename in os.listdir(research.name)) is (param in [1, 3])
                     assert (n_files == len(research.results.configs)) is (param in [2, 3])
 
                 if param in [True, 1, 3]:
                     if dump_results:
-                        with open(os.path.join(research.name, filename)) as file:
+                        with open(os.path.join(research.name, filename), encoding='utf-8') as file:
                             lines = ''.join(file.readlines())
                     else:
                         lines = list(getattr(research.storage, 'experiments_'+name).values())[0]
                     assert lines == output * 2
 
                 if dump_results and param in [2, 3]:
                     for full_path in research.results.artifacts_to_df(name=filename)['full_path']:
-                        with open(full_path) as file:
+                        with open(full_path, encoding='utf-8') as file:
                             lines = ''.join(file.readlines())
                             assert lines == output * 2
 
     def test_domain_with_objects(self, tmp_path):
         domain = Domain(a=[print, Research])
         research = Research(domain=domain).add_callable(lambda: 1)
         research.run(name=os.path.join(tmp_path, 'research'), parallel=False)
```

### Comparing `batchflow-0.8.1/batchflow/tests/save_to_test.py` & `batchflow-0.8.1a0/batchflow/tests/save_to_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/test_loss_test.py` & `batchflow-0.8.1a0/batchflow/tests/test_loss_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/torch_layers_test.py` & `batchflow-0.8.1a0/batchflow/tests/torch_layers_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/torch_models_compile_test.py` & `batchflow-0.8.1a0/batchflow/tests/torch_models_compile_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/tests/torch_models_test.py` & `batchflow-0.8.1a0/batchflow/tests/torch_models_test.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/utils.py` & `batchflow-0.8.1a0/batchflow/utils.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/utils_notebook.py` & `batchflow-0.8.1a0/batchflow/utils_notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             cell_counter += 1
             cell_code_counter = 0
 
     code = '\n'.join(code_list)
 
     # Create temporal file with code, run pylint on it
     temp_name = os.path.splitext(path)[0] + '.py'
-    with open(temp_name, 'w') as temp_file:
+    with open(temp_name, 'w', encoding='utf-8') as temp_file:
         temp_file.write(code)
 
     pylint_stdout, pylint_stderr = lint.py_run(temp_name + options, return_std=True)
 
     errors = pylint_stderr.getvalue()
     report = pylint_stdout.getvalue()
     if errors:
@@ -303,15 +303,15 @@
         Whether to show individual device information.
         If 0 or False, then no information is displayed.
         If 1 or True, then display the value assigned to `CUDA_VISIBLE_DEVICES` variable.
         If 2, then display memory and process information for each device.
     raise_error : bool
         Whether to raise an exception if not enough devices are available.
     """
-    if 'CUDA_VISIBLE_DEVICES' in os.environ.keys():
+    if 'CUDA_VISIBLE_DEVICES' in os.environ:
         str_devices = os.environ["CUDA_VISIBLE_DEVICES"]
         warnings.warn(f'`CUDA_VISIBLE_DEVICES` is already set to "{str_devices}"!')
         return [int(d) for d in str_devices.split(',')]
 
     devices = get_available_gpus(n=n, min_free_memory=min_free_memory, max_processes=max_processes,
                                  verbose=(verbose==2), raise_error=raise_error)
     str_devices = ','.join(str(i) for i in devices)
```

### Comparing `batchflow-0.8.1/batchflow/utils_random.py` & `batchflow-0.8.1a0/batchflow/utils_random.py`

 * *Files identical despite different names*

### Comparing `batchflow-0.8.1/batchflow/utils_telegram.py` & `batchflow-0.8.1a0/batchflow/utils_telegram.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 import os
 import json
 import imghdr
 from uuid import uuid4
 from io import BytesIO
 from concurrent.futures import ThreadPoolExecutor
 
-from urllib3 import PoolManager
-
-
 
 class TelegramMessage:
     """ Class to send a message with text or image (either a matplotlib figure or path to photo) to a Telegram bot.
     On subsequent updates, the same message is edited to avoid clutter in notifications.
     By default, all messages are silent (with no notifications).
 
     All of Telegram updates are send with `urllib3`, with no usage of official Telegram Python API.
@@ -24,14 +21,19 @@
         - add the bot to a chat and send it a message such as `/start`
         - go to <https://api.telegram.org/bot`{token}`/getUpdates> to find out the `{chat_id}`
     """
     API = 'https://api.telegram.org/bot'
     USER_AGENT = 'Python Telegram Bot (https://github.com/python-telegram-bot/python-telegram-bot)'
 
     def __init__(self, token=None, chat_id=None, silent=True, content=None):
+        try:
+            from urllib3 import PoolManager
+        except ImportError as e:
+            raise ImportError("urllib3 is missing. Install batchflow[telegram]") from e
+
         # Connection
         self.token = token or os.getenv('TELEGRAM_TOKEN')
         self.chat_id = chat_id or os.getenv('TELEGRAM_CHAT_ID')
         if self.token is None or self.chat_id is None:
             raise ValueError('Supply `token` and `chat_id` or '
                              'set `TELEGRAM_TOKEN` and `TELEGRAM_CHAT_ID` environment variables!')
```

### Comparing `batchflow-0.8.1/batchflow/variables.py` & `batchflow-0.8.1a0/batchflow/variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 
 from .named_expr import eval_expr
 
 
 class Variable:
     """ Pipeline variable """
+    #pylint: disable=consider-using-with
     def __init__(self, name, default=None, lock=True, pipeline=None):
         self.name = name
         self.default = default
         self._lock = threading.Lock() if lock else None
         self.value = None
         self.initialize(pipeline=pipeline)
 
@@ -48,14 +49,15 @@
         """ Release lock """
         if self._lock:
             self._lock.release()
 
 
 class VariableDirectory:
     """ Storage for pipeline variables """
+    #pylint: disable=consider-using-with
     def __init__(self, strict=False):
         self.variables = {}
         self.strict = strict
         self._lock = threading.Lock()
 
     def __getstate__(self):
         state = self.__dict__.copy()
```

