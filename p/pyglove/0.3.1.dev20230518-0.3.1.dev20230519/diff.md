# Comparing `tmp/pyglove-0.3.1.dev20230518.tar.gz` & `tmp/pyglove-0.3.1.dev20230519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230518.tar", last modified: Thu May 18 08:06:25 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230519.tar", last modified: Fri May 19 08:06:23 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230518.tar` & `pyglove-0.3.1.dev20230519.tar`

### file list

```diff
@@ -1,188 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-18 08:06:22.000000 pyglove-0.3.1.dev20230518/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.008340 pyglove-0.3.1.dev20230518/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.012341 pyglove-0.3.1.dev20230518/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.012341 pyglove-0.3.1.dev20230518/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.016341 pyglove-0.3.1.dev20230518/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.020341 pyglove-0.3.1.dev20230518/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.024341 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.024341 pyglove-0.3.1.dev20230518/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.032342 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30587 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    74703 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.032342 pyglove-0.3.1.dev20230518/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.036342 pyglove-0.3.1.dev20230518/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48578 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    82873 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   110021 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.036342 pyglove-0.3.1.dev20230518/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.036342 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:06:25.012341 pyglove-0.3.1.dev20230518/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 08:06:24.000000 pyglove-0.3.1.dev20230518/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:06:25.044342 pyglove-0.3.1.dev20230518/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-18 08:06:08.000000 pyglove-0.3.1.dev20230518/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-19 08:06:21.000000 pyglove-0.3.1.dev20230519/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.266333 pyglove-0.3.1.dev20230519/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.266333 pyglove-0.3.1.dev20230519/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.266333 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.270333 pyglove-0.3.1.dev20230519/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.270333 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30859 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74985 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.270333 pyglove-0.3.1.dev20230519/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48921 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79219 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/setup.py
```

### Comparing `pyglove-0.3.1.dev20230518/LICENSE` & `pyglove-0.3.1.dev20230519/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/PKG-INFO` & `pyglove-0.3.1.dev20230519/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230518
+Version: 0.3.1.dev20230519
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230518/README.md` & `pyglove-0.3.1.dev20230519/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230519/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,23 +191,32 @@
     if hasattr(inspect, 'get_annotations'):
       annotations = inspect.get_annotations(cls)
     else:
       annotations = cls.__dict__.get('__annotations__', {})
 
     fields = []
     for attr_name, attr_annotation in annotations.items():
-      # We consider class-level attributes in upper cases non-fields even
-      # when they appear with annotations.
-      if attr_name.isupper() or attr_name.startswith('_'):
+      if attr_name == '__kwargs__':
+        # __kwargs__ is speical annotation for enabling keyword arguments.
+        key = pg_typing.StrKey()
+      elif not attr_name.isupper() and not attr_name.startswith('_'):
+        key = pg_typing.ConstStrKey(attr_name)
+      else:
+        # We consider class-level attributes in upper cases non-fields even
+        # when they appear with annotations.
+        key = None
+
+      if key is None:
         continue
-      field = pg_typing.create_field(
-          (attr_name, attr_annotation), accept_value_as_annotation=False)
-      attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
-      if attr_value != pg_typing.MISSING_VALUE:
-        field.value.set_default(attr_value)
+
+      field = pg_typing.Field.from_annotation(key, attr_annotation)
+      if isinstance(key, pg_typing.ConstStrKey):
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if attr_value != pg_typing.MISSING_VALUE:
+          field.value.set_default(attr_value)
       fields.append(field)
     return fields
 
   @classmethod
   def _on_schema_update(cls):
     """Triggers when the schema for the class has been updated."""
     # Update the default value for each field after schema is updated. This is
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,32 +211,33 @@
         # Forgot to call super().__init__ will trigger error.
         self.x = x
 
     with self.assertRaisesRegex(
         ValueError, '.* should call `super.*__init__`'):
       _ = B(1)
 
-  def test_infer_symbolic_fields_from_annotations(self):
+  def test_symbolic_fields_from_annotations(self):
 
     class A(Object):
       x: int
-      y: float = 0.0
+      y: typing.Annotated[float, 'field y'] = 0.0
       z = 2
       # P is upper-case, thus will not be treated as symbolic field.
       P: int = 1
       # _q starts with _, which will not be treated as symbolic field either.
       _q: int = 2
 
     self.assertEqual(
         list(A.schema.fields.keys()),
         ['x', 'y'])
 
     a = A(1)
     self.assertEqual(a.x, 1)
     self.assertEqual(a.y, 0.0)
+    self.assertEqual(A.schema.get_field('y').description, 'field y')
 
     a = A(2, y=1.0)
     self.assertEqual(a.x, 2)
     self.assertEqual(a.y, 1.0)
 
     class B(A):
       p: str = 'foo'
@@ -275,14 +276,23 @@
     self.assertEqual(d.x, 1)
     self.assertEqual(d.y, 1.0)
     self.assertEqual(d.q, 2)
     self.assertEqual(d.k, 3)
     self.assertEqual(d.e, 4)
     self.assertEqual(d.f, 5)
 
+    class E(Object):
+      __kwargs__: typing.Any
+      x: int
+
+    self.assertIsNotNone(E.schema.dynamic_field)
+    e = E(1, y=3)
+    self.assertEqual(e.x, 1)
+    self.assertEqual(e.y, 3)
+
   def test_update_of_default_values(self):
 
     class A(Object):
       x: int
 
     class B(A):
       x = 1
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,14 +339,17 @@
 
 # Type conversion.
 from pyglove.core.typing.type_conversion import register_converter
 from pyglove.core.typing.type_conversion import get_converter
 from pyglove.core.typing.type_conversion import get_first_applicable_converter
 from pyglove.core.typing.type_conversion import get_json_value_converter
 
+# Annotation conversion.
+import pyglove.core.typing.annotation_conversion
+
 # Interface for custom typing.
 from pyglove.core.typing.custom_typing import CustomTyping
 
 # Callable signature.
 from pyglove.core.typing.callable_signature import Argument
 from pyglove.core.typing.callable_signature import CallableType
 from pyglove.core.typing.callable_signature import Signature
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.core.typing.callable_ext."""
 
 import unittest
+from pyglove.core.typing import annotation_conversion   # pylint: disable=unused-import
 from pyglove.core.typing import callable_ext
-# Importing `value_specs` to make `ValueSpec.from_annotation` to work.
-from pyglove.core.typing import value_specs   # pylint: disable=unused-import
 
 
 class CallWithOptionalKeywordArgsTest(unittest.TestCase):
   """Tests for typing.CallWithOptionalKeywordArgs."""
 
   def test_function(self):
     """Test call with function."""
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """Tests for pyglove.core.typing.callable_signature."""
 
 import copy
 import inspect
 import unittest
 
+from pyglove.core.typing import annotation_conversion   # pylint: disable=unused-import
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import value_specs as vs
 
 
 class SignatureTest(unittest.TestCase):
   """Tests for `Signature` class."""
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
   @classmethod
   def from_annotation(
       cls,
       annotation: Any,
       auto_typing=False,
       accept_value_as_annotation=False) -> 'ValueSpec':
     """Gets a concrete ValueSpec from annotation."""
-    assert False, 'Overridden in `value_specs.py`.'
+    assert False, 'Overridden in `annotation_conversion.py`.'
 
 
 class Field(object_utils.Formattable):
   """Class that represents the definition of one or a group of attributes.
 
   ``Field`` is held by a :class:`pyglove.Schema` object for defining the
   name(s), the validation and transformation rules on its/their value(s) for a
@@ -579,14 +579,25 @@
     self._value = value_spec
     self._description = description
 
     if metadata and not isinstance(metadata, dict):
       raise ValueError('metadata must be a dict.')
     self._metadata = metadata or {}
 
+  @classmethod
+  def from_annotation(
+      cls,
+      key: Union[str, KeySpec],
+      annotation: Any,
+      description: Optional[str] = None,
+      metadata: Optional[Dict[str, Any]] = None,
+      auto_typing=True) -> 'Field':
+    """Gets a Field from annotation."""
+    assert False, 'Overridden in `annotation_conversion.py`.'
+
   @property
   def description(self) -> Optional[str]:
     """Description of this field."""
     return self._description
 
   def set_description(self, description: str) -> None:
     """Sets the description for this field."""
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import copy
 import inspect
 import sys
 from typing import Optional, Union, List
 import unittest
 
+from pyglove.core.typing import annotation_conversion  # pylint: disable=unused-import
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import custom_typing
 from pyglove.core.typing import key_specs as ks
 from pyglove.core.typing import typed_missing
 from pyglove.core.typing import value_specs as vs
 from pyglove.core.typing.class_schema import Field
 from pyglove.core.typing.class_schema import Schema
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.core.typing.class_schema_utils."""
 
 import unittest
 
 from pyglove.core import object_utils
+from pyglove.core.typing import annotation_conversion   # pylint: disable=unused-import
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import class_schema_utils
 from pyglove.core.typing import key_specs as ks
 from pyglove.core.typing import value_specs as vs
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Concrete value specifications for field definition."""
-import collections
 import copy
 import functools
 import inspect
 import numbers
 import re
 import sys
-import types
 import typing
 import __main__
 
 from pyglove.core import object_utils
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import key_specs
@@ -2226,140 +2224,25 @@
 
 
 def _any_if_no_annotation(annotation: typing.Any):
   """Returns typing.Any if annotation is MISSING_VALUE."""
   return typing.Any if annotation == MISSING_VALUE else annotation
 
 
-_NoneType = type(None)
-
-# UnionType is supported after 3.10.
-_UnionType = getattr(types, 'UnionType', None)  # pylint: disable=invalid-name
-
-
-def _from_default_value(
-    value: typing.Any,
-    set_default: bool = True) -> typing.Optional[ValueSpec]:
-  """Creates a value spec from a default value."""
-  if isinstance(value, (bool, int, float, str, dict)):
-    value_spec = _from_type_annotation(type(value), False)
-  elif isinstance(value, list):
-    value_spec = List(_from_default_value(value[0], False) if value else Any())
-  elif isinstance(value, tuple):
-    value_spec = Tuple([_from_default_value(elem, False) for elem in value])
-  elif inspect.isfunction(value) or isinstance(value, object_utils.Functor):
-    value_spec = Callable()
-  elif not isinstance(value, type):
-    value_spec = Object(type(value))
-  else:
-    value_spec = None
-
-  if value_spec and set_default:
-    value_spec.set_default(value)
-  return value_spec
-
-
-def _from_type_annotation(
-    annotation: typing.Any, accept_value_as_annotation: bool) -> ValueSpec:
-  """Creates a value spec from type annotation."""
-  if annotation is bool:
-    return Bool()
-  elif annotation is int:
-    return Int()
-  elif annotation is float:
-    return Float()
-  elif annotation is str:
-    return Str()
-  elif annotation is typing.Any:
-    return Any().annotate(annotation)
-
-  origin = typing.get_origin(annotation) or annotation
-  args = list(typing.get_args(annotation))
-
-  # Handling list.
-  if origin in (list, typing.List):
-    return List(_from_annotation(args[0], True)) if args else List(Any())
-  # Handling tuple.
-  elif origin in (tuple, typing.Tuple):
-    if args:
-      return Tuple([_from_annotation(arg, True) for arg in args])
-    else:
-      return Tuple(Any())
-  # Handle sequence.
-  elif origin in (collections.abc.Sequence,):
-    elem = _from_annotation(args[0], True) if args else Any()
-    return Union([List(elem), Tuple(elem)])
-  # Handling dict.
-  elif origin in (dict, typing.Dict, collections.abc.Mapping):
-    # TODO(daiyip): Handle dict schema according to the dict args.
-    return Dict()
-  # Handling union.
-  elif origin is typing.Union or (_UnionType and origin is _UnionType):
-    optional = _NoneType in args
-    if optional:
-      args.remove(_NoneType)
-    if len(args) == 1:
-      spec = _from_annotation(args[0], True)
-    else:
-      spec = Union([_from_annotation(x, True) for x in set(args)])
-    if optional:
-      spec = spec.noneable()
-    return spec
-  # Handling class.
-  elif (inspect.isclass(annotation)
-        or (isinstance(annotation, str) and not accept_value_as_annotation)):
-    return Object(annotation)
-
-  if accept_value_as_annotation:
-    spec = _from_default_value(annotation)
-    if spec is not None:
-      return spec
-  raise TypeError(
-      f'Cannot convert {annotation!r} to `pg.typing.ValueSpec` '
-      f'with auto typing.')
-
-
-def _any_spec_with_annotation(annotation: typing.Any) -> Any:
-  """Creates an ``Any`` value spec with annotation."""
-  value_spec = Any()
-  if annotation != inspect.Parameter.empty:
-    value_spec.annotate(annotation)
-  return value_spec
-
-
-def _from_annotation(annotation: typing.Any,
-                     auto_typing=False,
-                     accept_value_as_annotation=False) -> ValueSpec:
-  """Creates a value spec from annotation."""
-  if isinstance(annotation, ValueSpec):
-    return annotation
-  elif annotation == inspect.Parameter.empty:
-    return Any()
-  elif annotation is None:
-    if accept_value_as_annotation:
-      return Any().noneable()
-    else:
-      return Any().freeze(None)
-
-  if auto_typing:
-    return _from_type_annotation(annotation, accept_value_as_annotation)
-  else:
-    value_spec = None
-    if accept_value_as_annotation:
-      # Accept default values is applicable only when auto typing is off.
-      value_spec = _from_default_value(annotation)
-    return value_spec or _any_spec_with_annotation(annotation)
+# We need to figure out the source file when a ForwardRef is created.
+# This is where a `ValueSpec` is created. It could be from direct construction
+# of the value spec object or calling from_annotation.
+_VALUE_SPEC_CREATION_ROOT_SITES = [
+    'pyglove/core/typing/value_specs.py',
+    'pyglove/core/typing/annotation_conversion.py',
+]
 
 
 def _get_spec_callsite_module():
   """Returns the module of the callsite where ValueSpec objects are created."""
   calling_module = None
   callstack = inspect.stack()
-  current_source_file = sys.modules[__name__].__file__
   for frame, file, *_ in callstack[1:]:
-    if file != current_source_file:
+    if all(not file.endswith(site) for site in _VALUE_SPEC_CREATION_ROOT_SITES):
       calling_module = inspect.getmodule(frame)
       break
   return calling_module or __main__
-
-
-ValueSpec.from_annotation = _from_annotation
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.core.typing.value_specs."""
 
 import contextlib
-import inspect
 import sys
 import typing
 import unittest
 
 from pyglove.core import object_utils
+from pyglove.core.typing import annotation_conversion   # pylint: disable=unused-import
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import typed_missing
 from pyglove.core.typing import value_specs as vs
-from pyglove.core.typing.class_schema import ValueSpec
 
 
 class BoolTest(unittest.TestCase):
   """Tests for `Bool`."""
 
   def test_value_type(self):
     self.assertEqual(vs.Bool().value_type, bool)
@@ -2914,176 +2913,14 @@
       vs.Any().extend(v)
 
     with self.assertRaisesRegex(
         ValueError, 'Cannot freeze .* without a default value.'):
       vs.Any().freeze()
 
 
-class FromAnnotationTest(unittest.TestCase):
-  """Tests for ValueSpec.fromAnnotation."""
-
-  def assert_from_annotation_with_default_value(self, annotation, expected):
-    self.assertEqual(
-        ValueSpec.from_annotation(annotation, accept_value_as_annotation=True),
-        expected)
-
-  def test_from_values(self):
-    self.assert_from_annotation_with_default_value(1, vs.Int(1))
-    self.assert_from_annotation_with_default_value(1.0, vs.Float(1.0))
-    self.assert_from_annotation_with_default_value(False, vs.Bool(False))
-    self.assert_from_annotation_with_default_value('abc', vs.Str('abc'))
-    self.assert_from_annotation_with_default_value(
-        [], vs.List(vs.Any(), default=[]))
-    self.assert_from_annotation_with_default_value(
-        [1, 2], vs.List(vs.Int(), default=[1, 2]))
-    self.assert_from_annotation_with_default_value(
-        {}, vs.Dict().set_default({}))
-    self.assert_from_annotation_with_default_value(
-        (1, 1.0, 'b'),
-        vs.Tuple([vs.Int(), vs.Float(), vs.Str()]).set_default((1, 1.0, 'b')))
-
-    class A:
-      pass
-
-    a = A()
-    self.assert_from_annotation_with_default_value(
-        a,
-        vs.Object(A, default=a))
-
-    f = lambda: 0
-    self.assert_from_annotation_with_default_value(
-        f,
-        vs.Callable(default=f))
-
-    with self.assertRaisesRegex(TypeError, 'Cannot convert .*'):
-      _ = ValueSpec.from_annotation(1, auto_typing=True)
-
-  def test_no_annotation(self):
-    self.assertEqual(
-        ValueSpec.from_annotation(inspect.Parameter.empty, False), vs.Any())
-    self.assertEqual(
-        ValueSpec.from_annotation(inspect.Parameter.empty, True), vs.Any())
-
-  def test_none(self):
-    self.assertEqual(
-        ValueSpec.from_annotation(None, False), vs.Any().freeze(None))
-    self.assertEqual(
-        ValueSpec.from_annotation(None, True), vs.Any().freeze(None))
-    self.assertEqual(
-        ValueSpec.from_annotation(
-            None, accept_value_as_annotation=True), vs.Any().noneable())
-
-  def test_any(self):
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Any, False),
-        vs.Any(annotation=typing.Any))
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Any, True),
-        vs.Any(annotation=typing.Any))
-
-  def test_bool(self):
-    self.assertEqual(ValueSpec.from_annotation(bool, True), vs.Bool())
-    self.assertEqual(
-        ValueSpec.from_annotation(bool, False), vs.Any(annotation=bool))
-    self.assertEqual(
-        ValueSpec.from_annotation(bool, False, True), vs.Any(annotation=bool))
-
-  def test_int(self):
-    self.assertEqual(ValueSpec.from_annotation(int, True), vs.Int())
-    self.assertEqual(ValueSpec.from_annotation(int, True, True), vs.Int())
-    self.assertEqual(
-        ValueSpec.from_annotation(int, False), vs.Any(annotation=int))
-    self.assertEqual(
-        ValueSpec.from_annotation(int, False, True), vs.Any(annotation=int))
-
-  def test_float(self):
-    self.assertEqual(ValueSpec.from_annotation(float, True), vs.Float())
-    self.assertEqual(ValueSpec.from_annotation(float, True, False), vs.Float())
-    self.assertEqual(
-        ValueSpec.from_annotation(float, False), vs.Any(annotation=float))
-    self.assertEqual(
-        ValueSpec.from_annotation(float, False, True), vs.Any(annotation=float))
-
-  def test_str(self):
-    self.assertEqual(ValueSpec.from_annotation(str, True), vs.Str())
-    self.assertEqual(ValueSpec.from_annotation(str, True, False), vs.Str())
-    self.assertEqual(
-        ValueSpec.from_annotation(str, False), vs.Any(annotation=str))
-    self.assertEqual(
-        ValueSpec.from_annotation(str, False, True), vs.Any(annotation=str))
-
-    self.assertEqual(
-        ValueSpec.from_annotation('A', False, False), vs.Any(annotation='A'))
-    self.assertEqual(
-        ValueSpec.from_annotation('A', False, True), vs.Str('A'))
-    self.assertEqual(
-        ValueSpec.from_annotation('A', True), vs.Object('A'))
-    self.assertEqual(
-        ValueSpec.from_annotation('A', True, True), vs.Str('A'))
-
-  def test_list(self):
-    self.assertEqual(ValueSpec.from_annotation(list, True), vs.List(vs.Any()))
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.List, True), vs.List(vs.Any()))
-    self.assertEqual(
-        ValueSpec.from_annotation(list[int], True), vs.List(vs.Int()))
-
-  def test_tuple(self):
-    self.assertEqual(ValueSpec.from_annotation(tuple, True), vs.Tuple(vs.Any()))
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Tuple, True), vs.Tuple(vs.Any()))
-    self.assertEqual(
-        ValueSpec.from_annotation(tuple[int], True), vs.Tuple([vs.Int()]))
-
-  def test_sequence(self):
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Sequence[int], True),
-        vs.Union([vs.List(vs.Int()), vs.Tuple(vs.Int())]))
-
-  def test_dict(self):
-    self.assertEqual(ValueSpec.from_annotation(dict, True), vs.Dict())
-    self.assertEqual(ValueSpec.from_annotation(typing.Dict, True), vs.Dict())
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Dict[str, int], True), vs.Dict())
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Mapping[str, int], True), vs.Dict())
-
-  def test_class(self):
-    class Foo:
-      pass
-
-    self.assertEqual(
-        ValueSpec.from_annotation(Foo, True), vs.Object(Foo))
-    self.assertEqual(
-        ValueSpec.from_annotation('Foo', True), vs.Object('Foo'))
-    self.assertEqual(
-        ValueSpec.from_annotation(Foo, False), vs.Any(annotation=Foo))
-
-  def test_optional(self):
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Optional[int], True),
-        vs.Int().noneable())
-    if vs._UnionType:
-      self.assertEqual(
-          ValueSpec.from_annotation(int | None, True),
-          vs.Int().noneable())
-
-  def test_union(self):
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Union[int, str], True),
-        vs.Union([vs.Int(), vs.Str()]))
-    self.assertEqual(
-        ValueSpec.from_annotation(typing.Union[int, str, None], True),
-        vs.Union([vs.Int(), vs.Str()]).noneable())
-    if vs._UnionType:
-      self.assertEqual(
-          ValueSpec.from_annotation(int | str, True),
-          vs.Union([vs.Int(), vs.Str()]))
-
-
 @contextlib.contextmanager
 def simulate_forward_declaration(*module_level_symbols):
   try:
     for symbol in module_level_symbols:
       setattr(sys.modules[__name__], symbol.__name__, symbol)
     yield
   finally:
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230518/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230519/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230518
+Version: 0.3.1.dev20230519
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230518/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230519/pyglove.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,16 @@
 pyglove/core/tuning/early_stopping.py
 pyglove/core/tuning/local_backend.py
 pyglove/core/tuning/protocols.py
 pyglove/core/tuning/protocols_test.py
 pyglove/core/tuning/sample.py
 pyglove/core/tuning/sample_test.py
 pyglove/core/typing/__init__.py
+pyglove/core/typing/annotation_conversion.py
+pyglove/core/typing/annotation_conversion_test.py
 pyglove/core/typing/callable_ext.py
 pyglove/core/typing/callable_ext_test.py
 pyglove/core/typing/callable_signature.py
 pyglove/core/typing/callable_signature_test.py
 pyglove/core/typing/class_schema.py
 pyglove/core/typing/class_schema_test.py
 pyglove/core/typing/class_schema_utils.py
```

### Comparing `pyglove-0.3.1.dev20230518/setup.py` & `pyglove-0.3.1.dev20230519/setup.py`

 * *Files identical despite different names*

