# Comparing `tmp/truss-0.4.6rc2.tar.gz` & `tmp/truss-0.4.6rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.6rc2.tar", max compression
+gzip compressed data, was "truss-0.4.6rc3.tar", max compression
```

## Comparing `truss-0.4.6rc2.tar` & `truss-0.4.6rc3.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0     5483 2023-05-16 17:24:35.347353 truss-0.4.6rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-05-16 17:24:35.347353 truss-0.4.6rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-05-16 17:24:35.347353 truss-0.4.6rc2/LICENSE
--rw-r--r--   0        0        0     5958 2023-05-16 17:24:35.347353 truss-0.4.6rc2/README.md
--rw-r--r--   0        0        0     3316 2023-05-16 17:24:35.347353 truss-0.4.6rc2/ROADMAP.md
--rw-r--r--   0        0        0      625 2023-05-16 17:24:35.347353 truss-0.4.6rc2/context_builder.Dockerfile
--rw-r--r--   0        0        0     2244 2023-05-16 17:24:35.427355 truss-0.4.6rc2/pyproject.toml
--rw-r--r--   0        0        0      330 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/build.py
--rw-r--r--   0        0        0    10452 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/cli.py
--rw-r--r--   0        0        0     2813 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/constants.py
--rw-r--r--   0        0        0     1294 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5709 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4770 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-05-16 17:24:35.427355 truss-0.4.6rc2/truss/errors.py
--rw-r--r--   0        0        0      824 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/notebook.py
--rw-r--r--   0        0        0    11065 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1892 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/external_data_resolver.py
--rw-r--r--   0        0        0     1352 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0      593 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     5674 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      176 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     2233 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0     1854 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/context_builder_image_test/server.Dockerfile
--rw-r--r--   0        0        0       72 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/tests/__init__.py
--rw-r--r--   0        0        0    20835 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/tests/conftest.py
--rw-r--r--   0        0        0     1256 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-05-16 17:24:35.431355 truss-0.4.6rc2/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2157 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/server/common/test_external_resolver.py
--rw-r--r--   0        0        0     2038 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_build.py
--rw-r--r--   0        0        0     2359 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    33195 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/tests/test_validation.py
--rw-r--r--   0        0        0    12200 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/truss_config.py
--rw-r--r--   0        0        0     2845 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41070 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/truss_handle.py
--rw-r--r--   0        0        0     5428 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/types.py
--rw-r--r--   0        0        0      227 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/util/jinja.py
--rw-r--r--   0        0        0     2018 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/util/path.py
--rw-r--r--   0        0        0     2317 2023-05-16 17:24:35.435355 truss-0.4.6rc2/truss/validation.py
--rw-r--r--   0        0        0     7339 1970-01-01 00:00:00.000000 truss-0.4.6rc2/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-05-17 18:43:25.064890 truss-0.4.6rc3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-05-17 18:43:25.064890 truss-0.4.6rc3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-05-17 18:43:25.064890 truss-0.4.6rc3/LICENSE
+-rw-r--r--   0        0        0     5958 2023-05-17 18:43:25.064890 truss-0.4.6rc3/README.md
+-rw-r--r--   0        0        0     3316 2023-05-17 18:43:25.064890 truss-0.4.6rc3/ROADMAP.md
+-rw-r--r--   0        0        0      625 2023-05-17 18:43:25.064890 truss-0.4.6rc3/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2244 2023-05-17 18:43:25.156895 truss-0.4.6rc3/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/cli.py
+-rw-r--r--   0        0        0     2813 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5709 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4770 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1976 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     1686 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6565 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/notebook.py
+-rw-r--r--   0        0        0    11065 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/__init__.py
+-rw-r--r--   0        0        0     2170 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1849 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       82 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0     2616 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/docs/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0      237 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1892 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/external_data_resolver.py
+-rw-r--r--   0        0        0     1352 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0      593 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     3318 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     5511 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      416 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      733 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     5674 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      176 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     2327 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0      216 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0     2253 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/context_builder_image_test/server.Dockerfile
+-rw-r--r--   0        0        0       72 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0      669 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20835 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1256 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6937 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2157 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/server/common/test_external_resolver.py
+-rw-r--r--   0        0        0     2038 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_build.py
+-rw-r--r--   0        0        0     2359 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     2605 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    33226 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    12200 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_config.py
+-rw-r--r--   0        0        0     2845 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41070 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_handle.py
+-rw-r--r--   0        0        0     5428 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/types.py
+-rw-r--r--   0        0        0      227 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/jinja.py
+-rw-r--r--   0        0        0     2018 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/path.py
+-rw-r--r--   0        0        0     2317 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/validation.py
+-rw-r--r--   0        0        0     7339 1970-01-01 00:00:00.000000 truss-0.4.6rc3/PKG-INFO
```

### Comparing `truss-0.4.6rc2/CODE_OF_CONDUCT.md` & `truss-0.4.6rc3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/CONTRIBUTING.md` & `truss-0.4.6rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/LICENSE` & `truss-0.4.6rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/README.md` & `truss-0.4.6rc3/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/ROADMAP.md` & `truss-0.4.6rc3/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/context_builder.Dockerfile` & `truss-0.4.6rc3/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/pyproject.toml` & `truss-0.4.6rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.6rc2"
+version = "0.4.6rc3"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.6rc2/truss/blob/blob_backend_registry.py` & `truss-0.4.6rc3/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/blob/http_public_blob_backend.py` & `truss-0.4.6rc3/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/build.py` & `truss-0.4.6rc3/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/cli.py` & `truss-0.4.6rc3/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/constants.py` & `truss-0.4.6rc3/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/image_builder/image_builder.py` & `truss-0.4.6rc3/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.6rc3/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.6rc3/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/image_builder/util.py` & `truss-0.4.6rc3/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.6rc3/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/local_loader/train_local.py` & `truss-0.4.6rc3/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.6rc3/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/contexts/local_loader/utils.py` & `truss-0.4.6rc3/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/docker.py` & `truss-0.4.6rc3/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/environment_inference/requirements_inference.py` & `truss-0.4.6rc3/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/errors.py` & `truss-0.4.6rc3/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/local/local_config.py` & `truss-0.4.6rc3/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/local/local_config_handler.py` & `truss-0.4.6rc3/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_framework.py` & `truss-0.4.6rc3/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/__init__.py` & `truss-0.4.6rc3/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.6rc3/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/keras.py` & `truss-0.4.6rc3/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/lightgbm.py` & `truss-0.4.6rc3/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/mlflow.py` & `truss-0.4.6rc3/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/pytorch.py` & `truss-0.4.6rc3/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/sklearn.py` & `truss-0.4.6rc3/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_frameworks/xgboost.py` & `truss-0.4.6rc3/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/model_inference.py` & `truss-0.4.6rc3/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/patch/calc_patch.py` & `truss-0.4.6rc3/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/patch/dir_signature.py` & `truss-0.4.6rc3/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/patch/hash.py` & `truss-0.4.6rc3/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/patch/types.py` & `truss-0.4.6rc3/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/readme_generator.py` & `truss-0.4.6rc3/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/README.md.jinja` & `truss-0.4.6rc3/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/base.Dockerfile.jinja` & `truss-0.4.6rc3/truss/templates/base.Dockerfile.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 ARG PYVERSION={{config.python_version}}
 FROM {{base_image_name_and_tag}}
 
 {% block fail_fast %}
 RUN grep -w 'ID=debian\|ID_LIKE=debian' /etc/os-release || { echo "ERROR: Supplied base image is not a debian image"; exit 1; }
-RUN which python && python --version | grep -E '3\.[0-9]|10\.[0-9][0-9]' || \
-    which python3 && python3 --version | grep -E '3\.[0-9]|10\.[0-9][0-9]' || \
-    { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.10"; exit 1; }
+RUN pythonVersion=$(echo $(command -v python >/dev/null 2>&1 && python --version || python3 --version) | cut -d" " -f2 | cut -d"." -f1,2) \
+    && echo $pythonVersion | grep -E '3\.[0-9]|10\.[0-9][0-9]' \
+    && apt-get update && ( apt-get install -y --no-install-recommends python$pythonVersion-venv || apt-get install -y --no-install-recommends python3-venv )  \
+    && apt-get autoremove -y \
+    && apt-get clean -y \
+    && rm -rf /var/lib/apt/lists/* \
+    || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.10"; exit 1; }
 {% endblock %}
 
 RUN pip install --upgrade pip --no-cache-dir \
     && rm -rf /root/.cache/pip
 
 {% block base_image_patch %}
 {% endblock %}
```

### Comparing `truss-0.4.6rc2/truss/templates/control/control/application.py` & `truss-0.4.6rc3/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/endpoints.py` & `truss-0.4.6rc3/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/helpers/errors.py` & `truss-0.4.6rc3/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.6rc3/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/helpers/types.py` & `truss-0.4.6rc3/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/control/control/server.py` & `truss-0.4.6rc3/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/custom/model/model.py` & `truss-0.4.6rc3/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/docs/README.md` & `truss-0.4.6rc3/truss/templates/docs/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.6rc3/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/keras/model/model.py` & `truss-0.4.6rc3/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/lightgbm/model/model.py` & `truss-0.4.6rc3/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/mlflow/model/model.py` & `truss-0.4.6rc3/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/pytorch/model/model.py` & `truss-0.4.6rc3/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/common/external_data_resolver.py` & `truss-0.4.6rc3/truss/templates/server/common/external_data_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/common/logging.py` & `truss-0.4.6rc3/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/common/retry.py` & `truss-0.4.6rc3/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/common/serialization.py` & `truss-0.4.6rc3/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/common/truss_server.py` & `truss-0.4.6rc3/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/inference_server.py` & `truss-0.4.6rc3/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server/model_wrapper.py` & `truss-0.4.6rc3/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/server.Dockerfile.jinja` & `truss-0.4.6rc3/truss/templates/server.Dockerfile.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 RUN apt update && \
     apt install -y bash \
                 build-essential \
                 git \
                 curl \
                 ca-certificates \
-                software-properties-common
+                software-properties-common \
+    && apt-get autoremove -y \
+    && apt-get clean -y \
+    && rm -rf /var/lib/apt/lists/*
 
 COPY ./base_server_requirements.txt base_server_requirements.txt
 RUN pip install -r base_server_requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
 
 # This is a hack, kfserving uses table_logger, which doesn't work well with
 # numpy 1.24 onwards, where np.float and np.int have been remove.
 # https://github.com/AleksTk/table-logger/blob/v0.3.6/table_logger/table_logger.py#L80
```

### Comparing `truss-0.4.6rc2/truss/templates/shared/secrets_resolver.py` & `truss-0.4.6rc3/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/sklearn/model/model.py` & `truss-0.4.6rc3/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/training/job.py` & `truss-0.4.6rc3/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/templates/xgboost/model/model.py` & `truss-0.4.6rc3/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/auto-mpg.data` & `truss-0.4.6rc3/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/context_builder_image_test/server.Dockerfile` & `truss-0.4.6rc3/truss/test_data/context_builder_image_test/server.Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 ARG PYVERSION=py39
 FROM baseten/truss-server-base:3.9-v0.4.3
 
 RUN grep -w 'ID=debian\|ID_LIKE=debian' /etc/os-release || { echo "ERROR: Supplied base image is not a debian image"; exit 1; }
-RUN which python && python --version | grep -E '3\.[0-9]|10\.[0-9][0-9]' || \
-    which python3 && python3 --version | grep -E '3\.[0-9]|10\.[0-9][0-9]' || \
-    { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.10"; exit 1; }
+RUN pythonVersion=$(echo $(command -v python >/dev/null 2>&1 && python --version || python3 --version) | cut -d" " -f2 | cut -d"." -f1,2) \
+    && echo $pythonVersion | grep -E '3\.[0-9]|10\.[0-9][0-9]' \
+    && apt-get update && ( apt-get install -y --no-install-recommends python$pythonVersion-venv || apt-get install -y --no-install-recommends python3-venv )  \
+    && apt-get autoremove -y \
+    && apt-get clean -y \
+    && rm -rf /var/lib/apt/lists/* \
+    || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.10"; exit 1; }
+
 
 RUN pip install --upgrade pip --no-cache-dir \
     && rm -rf /root/.cache/pip
 
 # If user base image is supplied in config, apply build commands from truss base image
 ENV PYTHONUNBUFFERED True
 ENV DEBIAN_FRONTEND=noninteractive
 
 RUN apt update && \
     apt install -y bash \
                 build-essential \
                 git \
                 curl \
                 ca-certificates \
-                software-properties-common
+                software-properties-common \
+    && apt-get autoremove -y \
+    && apt-get clean -y \
+    && rm -rf /var/lib/apt/lists/*
 
 COPY ./base_server_requirements.txt base_server_requirements.txt
 RUN pip install -r base_server_requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
 
 # This is a hack, kfserving uses table_logger, which doesn't work well with
 # numpy 1.24 onwards, where np.float and np.int have been remove.
 # https://github.com/AleksTk/table-logger/blob/v0.3.6/table_logger/table_logger.py#L80
```

### Comparing `truss-0.4.6rc2/truss/test_data/happy.ipynb` & `truss-0.4.6rc3/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.6rc3/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.6rc3/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/readme_int_example.md` & `truss-0.4.6rc3/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/readme_no_example.md` & `truss-0.4.6rc3/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/readme_str_example.md` & `truss-0.4.6rc3/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/test_truss/config.yaml` & `truss-0.4.6rc3/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/test_data/test_truss/model/model.py` & `truss-0.4.6rc3/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/conftest.py` & `truss-0.4.6rc3/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.4.6rc3/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.6rc3/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.6rc3/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.6rc3/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/local/test_local_config_handler.py` & `truss-0.4.6rc3/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.6rc3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.6rc3/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.6rc3/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.6rc3/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.6rc3/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.6rc3/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/patch/test_calc_patch.py` & `truss-0.4.6rc3/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/patch/test_hash.py` & `truss-0.4.6rc3/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/samples.py` & `truss-0.4.6rc3/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.6rc3/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/control/control/test_server.py` & `truss-0.4.6rc3/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.6rc3/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.6rc3/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/server/common/test_external_resolver.py` & `truss-0.4.6rc3/truss/tests/templates/server/common/test_external_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/server/common/test_retry.py` & `truss-0.4.6rc3/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.4.6rc3/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_backward.py` & `truss-0.4.6rc3/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_build.py` & `truss-0.4.6rc3/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_config.py` & `truss-0.4.6rc3/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_context_builder_image.py` & `truss-0.4.6rc3/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_docker.py` & `truss-0.4.6rc3/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_model_inference.py` & `truss-0.4.6rc3/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_notebooks.py` & `truss-0.4.6rc3/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.6rc3/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_truss_gatherer.py` & `truss-0.4.6rc3/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/tests/test_truss_handle.py` & `truss-0.4.6rc3/truss/tests/test_truss_handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,25 +95,26 @@
 
 
 @pytest.mark.integration
 @pytest.mark.parametrize(
     "base_image, expected_fail",
     [
         ("baseten/truss-server-base:3.9-v0.4.3", False),
-        ("python:3.8.3", False),
+        ("python:3.8", False),
         ("alpine", True),
         ("python:2.7-slim", True),
         ("python:3.5-slim", True),
     ],
 )
-def test_build_serving_docker_image_from_user_base_image(
+def test_build_serving_docker_image_from_user_base_image_live_reload(
     custom_model_truss_dir, base_image, expected_fail
 ):
     th = TrussHandle(custom_model_truss_dir)
     th.set_base_image(base_image)
+    th.live_reload()
     try:
         th.build_serving_docker_image(cache=False)
     except DockerException as exc:
         assert expected_fail is True
         assert "It returned with code 1" in str(exc)
```

### Comparing `truss-0.4.6rc2/truss/tests/test_validation.py` & `truss-0.4.6rc3/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/truss_config.py` & `truss-0.4.6rc3/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/truss_gatherer.py` & `truss-0.4.6rc3/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/truss_handle.py` & `truss-0.4.6rc3/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/truss_spec.py` & `truss-0.4.6rc3/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/types.py` & `truss-0.4.6rc3/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/util/gpu.py` & `truss-0.4.6rc3/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/util/path.py` & `truss-0.4.6rc3/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/truss/validation.py` & `truss-0.4.6rc3/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc2/PKG-INFO` & `truss-0.4.6rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.6rc2
+Version: 0.4.6rc3
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.11
```

