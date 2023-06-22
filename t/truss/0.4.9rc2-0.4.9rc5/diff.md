# Comparing `tmp/truss-0.4.9rc2.tar.gz` & `tmp/truss-0.4.9rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.9rc2.tar", max compression
+gzip compressed data, was "truss-0.4.9rc5.tar", max compression
```

## Comparing `truss-0.4.9rc2.tar` & `truss-0.4.9rc5.tar`

### file list

```diff
@@ -1,178 +1,184 @@
--rw-r--r--   0        0        0     5483 2023-06-13 20:41:33.831349 truss-0.4.9rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-06-13 20:41:33.831349 truss-0.4.9rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-06-13 20:41:33.831349 truss-0.4.9rc2/LICENSE
--rw-r--r--   0        0        0     5958 2023-06-13 20:41:33.831349 truss-0.4.9rc2/README.md
--rw-r--r--   0        0        0     3077 2023-06-13 20:41:33.831349 truss-0.4.9rc2/ROADMAP.md
--rw-r--r--   0        0        0      820 2023-06-13 20:41:33.835349 truss-0.4.9rc2/context_builder.Dockerfile
--rw-r--r--   0        0        0     2482 2023-06-13 20:41:33.939350 truss-0.4.9rc2/pyproject.toml
--rw-r--r--   0        0        0      330 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-06-13 20:41:33.939350 truss-0.4.9rc2/truss/build.py
--rw-r--r--   0        0        0    11326 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/cli.py
--rw-r--r--   0        0        0     2813 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/constants.py
--rw-r--r--   0        0        0     1294 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     8411 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2111 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     4715 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/local_server_loader.py
--rw-r--r--   0        0        0     2239 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0      951 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/truss_file_syncer.py
--rw-r--r--   0        0        0     5801 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/errors.py
--rw-r--r--   0        0        0      824 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6521 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/notebook.py
--rw-r--r--   0        0        0    11065 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/__init__.py
--rw-r--r--   0        0        0     1925 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2503 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4272 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     3015 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2450 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     1352 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/logging.py
--rw-r--r--   0        0        0     5389 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1875 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      126 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.943350 truss-0.4.9rc2/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     2382 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     9977 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0     1445 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      727 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0      496 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/local_inference_server.py
--rw-r--r--   0        0        0     6219 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      250 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     2769 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0      739 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/__init__.py
--rw-r--r--   0        0        0    20811 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-06-13 20:41:33.947350 truss-0.4.9rc2/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6977 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_build.py
--rw-r--r--   0        0        0     3181 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_docker.py
--rw-r--r--   0        0        0     7062 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    33928 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/tests/test_validation.py
--rw-r--r--   0        0        0    13164 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_config.py
--rw-r--r--   0        0        0     2698 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41382 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/types.py
--rw-r--r--   0        0        0      227 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/jinja.py
--rw-r--r--   0        0        0     2612 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-06-13 20:41:33.951350 truss-0.4.9rc2/truss/validation.py
--rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 truss-0.4.9rc2/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-06-16 19:49:28.511391 truss-0.4.9rc5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-06-16 19:49:28.511391 truss-0.4.9rc5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-06-16 19:49:28.511391 truss-0.4.9rc5/LICENSE
+-rw-r--r--   0        0        0     5958 2023-06-16 19:49:28.511391 truss-0.4.9rc5/README.md
+-rw-r--r--   0        0        0      933 2023-06-16 19:49:28.511391 truss-0.4.9rc5/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2482 2023-06-16 19:49:28.623398 truss-0.4.9rc5/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/build.py
+-rw-r--r--   0        0        0    11326 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/cli.py
+-rw-r--r--   0        0        0     2813 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     8411 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2111 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     4715 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/local_server_loader.py
+-rw-r--r--   0        0        0     2239 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0      951 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     5565 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/notebook.py
+-rw-r--r--   0        0        0    10744 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/signature.py
+-rw-r--r--   0        0        0     3087 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      937 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1925 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2559 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4272 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5859 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     3015 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2450 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     1352 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/logging.py
+-rw-r--r--   0        0        0      998 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     4483 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     3070 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1875 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      126 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1352 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     2382 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     3318 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     9977 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0     1445 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      727 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0      496 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/local_inference_server.py
+-rw-r--r--   0        0        0     6219 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      250 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     2769 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20811 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     1929 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     2065 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     6977 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_build.py
+-rw-r--r--   0        0        0     3181 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     7062 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    33928 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    13164 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41382 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/types.py
+-rw-r--r--   0        0        0      227 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/jinja.py
+-rw-r--r--   0        0        0     2612 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/validation.py
+-rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 truss-0.4.9rc5/PKG-INFO
```

### Comparing `truss-0.4.9rc2/CODE_OF_CONDUCT.md` & `truss-0.4.9rc5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/CONTRIBUTING.md` & `truss-0.4.9rc5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/LICENSE` & `truss-0.4.9rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/README.md` & `truss-0.4.9rc5/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/context_builder.Dockerfile` & `truss-0.4.9rc5/context_builder.Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,16 @@
     && apt-get autoremove -y \
     && apt-get clean -y \
     && rm -rf /var/lib/apt/lists/* /tmp/library-scripts/
 
 RUN curl -sSL https://install.python-poetry.org | python -
 
 ENV PATH="/root/.local/bin:${PATH}"
-COPY . .
+COPY ./truss ./truss
+COPY ./pyproject.toml ./pyproject.toml
+COPY ./poetry.lock ./poetry.lock
+COPY ./README.md ./README.md
 
 # https://python-poetry.org/docs/configuration/#virtualenvsin-project
 # to write to project root .venv file to be used for context builder test
 RUN poetry config virtualenvs.in-project true \
     && poetry install --only builder
```

### Comparing `truss-0.4.9rc2/pyproject.toml` & `truss-0.4.9rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.9rc2"
+version = "0.4.9rc5"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.9rc2/truss/blob/blob_backend_registry.py` & `truss-0.4.9rc5/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/blob/http_public_blob_backend.py` & `truss-0.4.9rc5/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/build.py` & `truss-0.4.9rc5/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/cli.py` & `truss-0.4.9rc5/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/constants.py` & `truss-0.4.9rc5/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/image_builder/image_builder.py` & `truss-0.4.9rc5/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.9rc5/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.9rc5/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/image_builder/util.py` & `truss-0.4.9rc5/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.4.9rc5/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.9rc5/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/local_server_loader.py` & `truss-0.4.9rc5/truss/contexts/local_loader/local_server_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/train_local.py` & `truss-0.4.9rc5/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/truss_file_syncer.py` & `truss-0.4.9rc5/truss/contexts/local_loader/truss_file_syncer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.9rc5/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/contexts/local_loader/utils.py` & `truss-0.4.9rc5/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/docker.py` & `truss-0.4.9rc5/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/environment_inference/requirements_inference.py` & `truss-0.4.9rc5/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/errors.py` & `truss-0.4.9rc5/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/local/local_config.py` & `truss-0.4.9rc5/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/local/local_config_handler.py` & `truss-0.4.9rc5/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_framework.py` & `truss-0.4.9rc5/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/__init__.py` & `truss-0.4.9rc5/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.9rc5/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/keras.py` & `truss-0.4.9rc5/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/lightgbm.py` & `truss-0.4.9rc5/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/mlflow.py` & `truss-0.4.9rc5/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/pytorch.py` & `truss-0.4.9rc5/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/sklearn.py` & `truss-0.4.9rc5/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_frameworks/xgboost.py` & `truss-0.4.9rc5/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/model_inference.py` & `truss-0.4.9rc5/truss/model_inference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import inspect
 import logging
-import pathlib
 import sys
 from ast import ClassDef, FunctionDef
 from dataclasses import dataclass
 from typing import Any, Dict, List, Tuple
 
-import pkg_resources  # type: ignore
-from pkg_resources.extern.packaging import requirements  # type: ignore
 from truss.constants import (
     HUGGINGFACE_TRANSFORMER,
     KERAS,
     LIGHTGBM,
     PYTORCH,
     SKLEARN,
     TENSORFLOW,
@@ -114,35 +111,14 @@
 
     return ModelBuildStageOne(
         model_type,
         model_framework,
     )
 
 
-def parse_requirements_file(requirements_file: str) -> dict:
-    name_to_req_str = {}
-    with pathlib.Path(requirements_file).open() as reqs_file:
-        for raw_req in reqs_file.readlines():
-            try:
-                req = pkg_resources.Requirement.parse(raw_req)
-                if req.specifier:  # type: ignore
-                    name_to_req_str[req.name] = str(req)  # type: ignore
-                else:
-                    name_to_req_str[str(req)] = str(req)
-            except requirements.InvalidRequirement:
-                # there might be pip requirements that do not conform
-                raw_req = str(raw_req).strip()
-                name_to_req_str[f"custom_{raw_req}"] = raw_req
-            except ValueError:
-                # can't parse empty lines
-                pass
-
-    return name_to_req_str
-
-
 def _infer_model_init_parameters(model_class: Any) -> Tuple[List, List]:
     full_arg_spec = inspect.getfullargspec(model_class.__init__)
     named_args = full_arg_spec.args[1:]
     number_of_kwargs = full_arg_spec.defaults and len(full_arg_spec.defaults) or 0
     required_args = full_arg_spec.args[1:-number_of_kwargs]
     return named_args, required_args
```

### Comparing `truss-0.4.9rc2/truss/patch/calc_patch.py` & `truss-0.4.9rc5/truss/patch/calc_patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import logging
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set
+from typing import Dict, List, Optional, Set
 
-import pkg_resources
 import yaml
 from truss.constants import CONFIG_FILE
 from truss.patch.hash import file_content_hash_str
 from truss.patch.types import TrussSignature
+from truss.templates.control.control.helpers.truss_patch.requirement_name_identifier import (
+    reqs_by_name,
+)
+from truss.templates.control.control.helpers.truss_patch.system_packages import (
+    system_packages_set,
+)
 from truss.templates.control.control.helpers.types import (
     Action,
     ModelCodePatch,
     Patch,
     PatchType,
     PythonRequirementPatch,
     SystemPackagePatch,
@@ -206,74 +211,55 @@
 ) -> List[Patch]:
     """Calculate patch based on changes to python requirements.
 
     Returns None if patch cannot be calculated. Empty list means no relevant
     differences found.
     """
     patches = []
-    prev_reqs = _parsed_reqs_by_name(prev_config.requirements)
+    prev_reqs = reqs_by_name(prev_config.requirements)
     prev_req_names = set(prev_reqs.keys())
-    new_reqs = _parsed_reqs_by_name(new_config.requirements)
+    new_reqs = reqs_by_name(new_config.requirements)
     new_req_names = set(new_reqs.keys())
     removed_reqs = prev_req_names.difference(new_req_names)
     for removed_req in removed_reqs:
         patches.append(_mk_python_requirement_patch(Action.REMOVE, removed_req))
 
     added_reqs = new_req_names.difference(prev_req_names)
     for added_req in added_reqs:
-        patches.append(
-            _mk_python_requirement_patch(Action.ADD, str(new_reqs[added_req]))
-        )
+        patches.append(_mk_python_requirement_patch(Action.ADD, new_reqs[added_req]))
 
     for req in new_req_names.intersection(prev_req_names):
         if new_reqs[req] != prev_reqs[req]:
-            patches.append(
-                _mk_python_requirement_patch(Action.UPDATE, str(new_reqs[req]))
-            )
+            patches.append(_mk_python_requirement_patch(Action.UPDATE, new_reqs[req]))
 
     return patches
 
 
 def _calc_system_packages_patches(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> List[Patch]:
     """Calculate patch based on changes to system packates.
 
     Returns None if patch cannot be calculated. Empty list means no relevant
     differences found.
     """
     patches = []
-    prev_pkgs = _system_pacakges_set(prev_config)
-    new_pkgs = _system_pacakges_set(new_config)
+    prev_pkgs = system_packages_set(prev_config.system_packages)
+    new_pkgs = system_packages_set(new_config.system_packages)
     removed_pkgs = prev_pkgs.difference(new_pkgs)
     for removed_pkg in removed_pkgs:
         patches.append(_mk_system_package_patch(Action.REMOVE, removed_pkg))
 
     added_pkgs = new_pkgs.difference(prev_pkgs)
     for added_pkg in added_pkgs:
         patches.append(_mk_system_package_patch(Action.ADD, added_pkg))
 
     return patches
 
 
-def _system_pacakges_set(config: TrussConfig) -> Set[str]:
-    pkgs = []
-    for sys_pkg_line in config.system_packages:
-        pkgs.extend(sys_pkg_line.strip().split())
-    return set(pkgs)
-
-
-def _parsed_reqs_by_name(reqs: List[str]) -> Dict[str, Any]:
-    parsed_reqs_by_name = {}
-    for req in reqs:
-        parsed_req = pkg_resources.Requirement.parse(req)
-        parsed_reqs_by_name[parsed_req.name] = parsed_req  # type: ignore
-    return parsed_reqs_by_name
-
-
 def _only_expected_config_differences(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> bool:
     prev_config_dict = prev_config.to_dict()
     prev_config_dict["requirements"] = []
     prev_config_dict["system_packages"] = []
```

### Comparing `truss-0.4.9rc2/truss/patch/dir_signature.py` & `truss-0.4.9rc5/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/patch/hash.py` & `truss-0.4.9rc5/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/patch/types.py` & `truss-0.4.9rc5/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/readme_generator.py` & `truss-0.4.9rc5/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/README.md.jinja` & `truss-0.4.9rc5/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/base.Dockerfile.jinja` & `truss-0.4.9rc5/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/application.py` & `truss-0.4.9rc5/truss/templates/control/control/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from endpoints import control_app
 from fastapi import FastAPI
 from fastapi.responses import JSONResponse
 from helpers.errors import ModelLoadFailed, PatchApplicatonError
 from helpers.inference_server_controller import InferenceServerController
 from helpers.inference_server_process_controller import InferenceServerProcessController
 from helpers.logging import setup_logging
-from helpers.patch_applier import PatchApplier
+from helpers.truss_patch.model_container_patch_applier import ModelContainerPatchApplier
 
 
 async def handle_patch_error(_, exc):
     error_type = _camel_to_snake_case(type(exc).__name__)
     return JSONResponse(
         content={
             "error": {
@@ -65,15 +65,15 @@
         app.state.inference_server_process_args,
         app.state.inference_server_port,
         app_logger=app_logger,
     )
 
     pip_path = getattr(app.state, "pip_path", None)
 
-    patch_applier = PatchApplier(
+    patch_applier = ModelContainerPatchApplier(
         Path(app.state.inference_server_home),
         app_logger,
         pip_path,
     )
 
     oversee_inference_server = getattr(app.state, "oversee_inference_server", True)
```

### Comparing `truss-0.4.9rc2/truss/templates/control/control/endpoints.py` & `truss-0.4.9rc5/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/errors.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 from helpers.errors import (
     InadmissiblePatch,
     PatchFailedRecoverable,
     PatchFailedUnrecoverable,
     UnsupportedPatch,
 )
 from helpers.inference_server_process_controller import InferenceServerProcessController
-from helpers.patch_applier import PatchApplier
+from helpers.truss_patch.model_container_patch_applier import ModelContainerPatchApplier
 from helpers.types import Patch, PatchType
 
 INFERENCE_SERVER_CHECK_INTERVAL_SECS = 10
 
 
 class InferenceServerController:
     """Controls what code the inference server runs with.
 
     Currently, it only applies locks to various actions and mostly
     delegates to InferenceServerProcessController.
     """
 
     _process_controller: InferenceServerProcessController
-    _patch_applier: PatchApplier
+    _patch_applier: ModelContainerPatchApplier
     _app_logger: logging.Logger
     _oversee_inference_server: bool
 
     def __init__(
         self,
         process_controller: InferenceServerProcessController,
-        patch_applier: PatchApplier,
+        patch_applier: ModelContainerPatchApplier,
         app_logger: logging.Logger,
         oversee_inference_server: bool = True,
     ):
         self._lock = threading.Lock()
         self._process_controller = process_controller
         self._patch_applier = patch_applier
         self._current_running_hash = os.environ.get("HASH_TRUSS", None)
@@ -82,15 +82,15 @@
                 raise UnsupportedPatch(str(exc)) from exc
 
             self._process_controller.stop()
             patches.sort(key=_patch_sort_key_fn)
             try:
                 patches_executed = 0
                 for patch in patches:
-                    self._patch_applier.apply_patch(patch)
+                    self._patch_applier(patch)
                     patches_executed += 1
             except Exception as exc:
                 if patches_executed > 0:
                     # In this case we leave inference server stopped, to reflect
                     # the bad state; with partially applied patch all bets are off.
                     # Correct handling of this scenario is to fallback to full deploy.
                     self._has_partially_applied_patch = True
```

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/logging.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,51 @@
+import logging
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 from helpers.errors import UnsupportedPatch
+from helpers.truss_patch.model_code_patch_applier import apply_model_code_patch
 from helpers.types import (
     Action,
     ModelCodePatch,
     Patch,
     PythonRequirementPatch,
     SystemPackagePatch,
 )
 from truss.truss_config import TrussConfig
 
 
-class PatchApplier:
+class ModelContainerPatchApplier:
+    """Applies patches to container running a truss.
+    This should be compatible with TrussDirPatchApplier.
+    """
+
     def __init__(
         self,
         inference_server_home: Path,
-        app_logger,
+        app_logger: logging.Logger,
         pip_path: Optional[str] = None,  # Only meant for testing
     ) -> None:
         self._inference_server_home = inference_server_home
         self._model_module_dir = (
             self._inference_server_home / self._truss_config.model_module_dir
         )
         self._app_logger = app_logger
         self._pip_path_cached = None
         if pip_path is not None:
             self._pip_path_cached = "pip"
 
-    def apply_patch(self, patch: Patch):
+    def __call__(self, patch: Patch):
         self._app_logger.debug(f"Applying patch {patch.to_dict()}")
         if isinstance(patch.body, ModelCodePatch):
             model_code_patch: ModelCodePatch = patch.body
-            self._apply_model_code_patch(model_code_patch)
+            apply_model_code_patch(
+                self._model_module_dir, model_code_patch, self._app_logger
+            )
         elif isinstance(patch.body, PythonRequirementPatch):
             py_req_patch: PythonRequirementPatch = patch.body
             self._apply_python_requirement_patch(py_req_patch)
         elif isinstance(patch.body, SystemPackagePatch):
             sys_pkg_patch: SystemPackagePatch = patch.body
             self._apply_system_package_patch(sys_pkg_patch)
         else:
@@ -49,42 +57,14 @@
 
     @property
     def _pip_path(self) -> str:
         if self._pip_path_cached is None:
             self._pip_path_cached = _identify_pip_path()
         return self._pip_path_cached
 
-    def _apply_model_code_patch(self, model_code_patch: ModelCodePatch):
-        self._app_logger.debug(
-            f"Applying model code patch {model_code_patch.to_dict()}"
-        )
-        action = model_code_patch.action
-        filepath: Path = self._model_module_dir / model_code_patch.path
-        if action in [Action.ADD, Action.UPDATE]:
-            filepath.parent.mkdir(parents=True, exist_ok=True)
-            self._app_logger.info(f"Updating file {filepath}")
-            with filepath.open("w") as file:
-                content = model_code_patch.content
-                if content is None:
-                    raise ValueError(
-                        "Invalid patch: content of a model code update patch should not be None."
-                    )
-                file.write(content)
-
-        elif action == Action.REMOVE:
-            if not filepath.exists():
-                self._app_logger.warning(
-                    f"Could not delete file {filepath}: not found."
-                )
-            else:
-                self._app_logger.info(f"Deleting file {filepath}")
-                filepath.unlink()
-        else:
-            raise ValueError(f"Unknown model code patch action {action}")
-
     def _apply_python_requirement_patch(
         self, python_requirement_patch: PythonRequirementPatch
     ):
         self._app_logger.debug(
             f"Applying python requirement patch {python_requirement_patch.to_dict()}"
         )
         action = python_requirement_patch.action
```

### Comparing `truss-0.4.9rc2/truss/templates/control/control/helpers/types.py` & `truss-0.4.9rc5/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/control/control/server.py` & `truss-0.4.9rc5/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/custom/model/model.py` & `truss-0.4.9rc5/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.9rc5/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/keras/model/model.py` & `truss-0.4.9rc5/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/lightgbm/model/model.py` & `truss-0.4.9rc5/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/mlflow/model/model.py` & `truss-0.4.9rc5/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/pytorch/model/model.py` & `truss-0.4.9rc5/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/errors.py` & `truss-0.4.9rc5/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/logging.py` & `truss-0.4.9rc5/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.4.9rc5/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/patches.py` & `truss-0.4.9rc5/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/retry.py` & `truss-0.4.9rc5/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/serialization.py` & `truss-0.4.9rc5/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/truss_server.py` & `truss-0.4.9rc5/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/common/util.py` & `truss-0.4.9rc5/truss/templates/server/common/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/inference_server.py` & `truss-0.4.9rc5/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server/model_wrapper.py` & `truss-0.4.9rc5/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/server.Dockerfile.jinja` & `truss-0.4.9rc5/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/shared/secrets_resolver.py` & `truss-0.4.9rc5/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/sklearn/model/model.py` & `truss-0.4.9rc5/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/training/job.py` & `truss-0.4.9rc5/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/templates/xgboost/model/model.py` & `truss-0.4.9rc5/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/auto-mpg.data` & `truss-0.4.9rc5/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/happy.ipynb` & `truss-0.4.9rc5/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/model_load_failure_test/config.yaml` & `truss-0.4.9rc5/truss/test_data/model_load_failure_test/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.4.9rc5/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.9rc5/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.9rc5/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/readme_int_example.md` & `truss-0.4.9rc5/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/readme_no_example.md` & `truss-0.4.9rc5/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/readme_str_example.md` & `truss-0.4.9rc5/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/server.Dockerfile` & `truss-0.4.9rc5/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/test_truss/config.yaml` & `truss-0.4.9rc5/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/test_data/test_truss/model/model.py` & `truss-0.4.9rc5/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/conftest.py` & `truss-0.4.9rc5/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.4.9rc5/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.9rc5/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.9rc5/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.9rc5/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/local/test_local_config_handler.py` & `truss-0.4.9rc5/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.9rc5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.9rc5/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.9rc5/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.9rc5/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.9rc5/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.9rc5/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/patch/test_calc_patch.py` & `truss-0.4.9rc5/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/patch/test_hash.py` & `truss-0.4.9rc5/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/samples.py` & `truss-0.4.9rc5/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,58 +11,66 @@
         / "templates"
         / "control"
         / "control"
     )
 )
 
 # Have to use imports in this form, otherwise isinstance checks fail on helper classes
-from helpers.patch_applier import PatchApplier  # noqa
+from helpers.truss_patch.model_container_patch_applier import (  # noqa
+    ModelContainerPatchApplier,
+)
 from helpers.types import Action, ModelCodePatch, Patch, PatchType  # noqa
 
 
 @pytest.fixture
 def patch_applier(truss_container_fs):
-    return PatchApplier(truss_container_fs / "app", Mock())
+    return ModelContainerPatchApplier(truss_container_fs / "app", Mock())
 
 
-def test_patch_applier_add(patch_applier: PatchApplier, truss_container_fs):
+def test_patch_applier_add(
+    patch_applier: ModelContainerPatchApplier, truss_container_fs
+):
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.ADD,
             path="dummy",
             content="",
         ),
     )
-    patch_applier.apply_patch(patch)
+    patch_applier(patch)
     assert (truss_container_fs / "app" / "model" / "dummy").exists()
 
 
-def test_patch_applier_remove(patch_applier: PatchApplier, truss_container_fs):
+def test_patch_applier_remove(
+    patch_applier: ModelContainerPatchApplier, truss_container_fs
+):
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.REMOVE,
             path="model.py",
         ),
     )
     assert (truss_container_fs / "app" / "model" / "model.py").exists()
-    patch_applier.apply_patch(patch)
+    patch_applier(patch)
     assert not (truss_container_fs / "app" / "model" / "model.py").exists()
 
 
-def test_patch_applier_update(patch_applier: PatchApplier, truss_container_fs):
+def test_patch_applier_update(
+    patch_applier: ModelContainerPatchApplier, truss_container_fs
+):
     new_model_file_content = """
     class Model:
         pass
     """
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="model.py",
             content=new_model_file_content,
         ),
     )
-    patch_applier.apply_patch(patch)
+    patch_applier(patch)
     with (truss_container_fs / "app" / "model" / "model.py").open() as model_file:
         assert model_file.read() == new_model_file_content
```

### Comparing `truss-0.4.9rc2/truss/tests/templates/control/control/test_server.py` & `truss-0.4.9rc5/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.9rc5/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.9rc5/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/templates/server/common/test_retry.py` & `truss-0.4.9rc5/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.4.9rc5/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_backward.py` & `truss-0.4.9rc5/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_build.py` & `truss-0.4.9rc5/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_config.py` & `truss-0.4.9rc5/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_context_builder_image.py` & `truss-0.4.9rc5/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_docker.py` & `truss-0.4.9rc5/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_model_inference.py` & `truss-0.4.9rc5/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_notebooks.py` & `truss-0.4.9rc5/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.9rc5/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_truss_gatherer.py` & `truss-0.4.9rc5/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_truss_handle.py` & `truss-0.4.9rc5/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/tests/test_validation.py` & `truss-0.4.9rc5/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/truss_config.py` & `truss-0.4.9rc5/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/truss_gatherer.py` & `truss-0.4.9rc5/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/truss_handle.py` & `truss-0.4.9rc5/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/truss_spec.py` & `truss-0.4.9rc5/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/types.py` & `truss-0.4.9rc5/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/util/gpu.py` & `truss-0.4.9rc5/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/util/path.py` & `truss-0.4.9rc5/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/truss/validation.py` & `truss-0.4.9rc5/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc2/PKG-INFO` & `truss-0.4.9rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.9rc2
+Version: 0.4.9rc5
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

