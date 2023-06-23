# Comparing `tmp/sparseml_nightly-1.6.0.20230616-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230623-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,374 +1,374 @@
-Zip file size: 959278 bytes, number of entries: 372
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-16 12:34 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-16 12:34 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-16 12:34 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-16 12:34 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-16 12:34 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-16 12:34 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-16 12:34 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-16 12:34 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-16 12:34 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-16 12:34 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-16 12:34 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-16 12:34 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-16 12:34 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-16 12:34 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-16 12:34 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-16 12:34 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     6058 b- defN 23-Jun-16 12:34 sparseml/exporters/kv_cache_injector.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-16 12:34 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2276 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4866 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4681 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/kv_cache/__init__.py
--rw-rw-r--  2.0 unx    20939 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
--rw-rw-r--  2.0 unx     6763 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx    10570 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-16 12:34 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-16 12:34 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-16 12:34 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-16 12:34 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-16 12:34 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-16 12:34 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jun-16 12:34 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-16 12:34 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-16 12:34 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-16 12:34 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-16 12:34 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-16 12:34 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-16 12:34 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-16 12:34 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-16 12:34 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-16 12:34 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-16 12:34 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-16 12:34 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-16 12:34 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-16 12:34 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jun-16 12:34 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-16 12:34 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jun-16 12:34 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-16 12:34 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-16 12:34 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-16 12:34 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-16 12:34 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-16 12:34 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-16 12:34 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-16 12:34 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-16 12:34 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-16 12:34 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-16 12:34 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-16 12:34 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14532 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-16 12:34 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-16 12:34 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-16 12:34 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-16 12:34 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jun-16 12:34 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-16 12:34 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-16 12:34 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-16 12:34 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-16 12:34 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-16 12:34 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-16 12:34 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6117 b- defN 23-Jun-16 12:34 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-16 12:34 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10864 b- defN 23-Jun-16 12:34 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-16 12:34 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jun-16 12:34 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-16 12:34 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20676 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-16 12:34 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-16 12:34 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-16 12:34 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-16 12:34 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-16 12:34 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    76796 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-16 12:34 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-16 12:34 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-16 12:34 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-16 12:34 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-16 12:34 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-16 12:34 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-16 12:34 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-16 12:34 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-16 12:34 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-16 12:34 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-16 12:34 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-16 12:34 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-16 12:34 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-16 12:34 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-16 12:34 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-16 12:34 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    21290 b- defN 23-Jun-16 12:34 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-16 12:34 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-16 12:34 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-16 12:34 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-16 12:34 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-16 12:34 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-16 12:34 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-16 12:34 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jun-16 12:34 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-16 12:34 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-16 12:34 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-16 12:34 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-16 12:34 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-16 12:34 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-16 12:34 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-16 12:34 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-16 12:34 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-16 12:34 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-16 12:34 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-16 12:34 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-16 12:34 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-16 12:34 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-16 12:34 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-16 12:34 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-16 12:34 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-16 12:34 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-16 12:34 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-16 12:34 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    34788 b- defN 23-Jun-16 12:34 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-16 12:34 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-16 12:34 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jun-16 12:34 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-16 12:34 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-16 12:34 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21650 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    37031 b- defN 23-Jun-16 12:36 sparseml_nightly-1.6.0.20230616.dist-info/RECORD
-372 files, 3471754 bytes uncompressed, 899318 bytes compressed:  74.1%
+Zip file size: 959522 bytes, number of entries: 372
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-23 01:31 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-23 01:31 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-23 01:31 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-23 01:31 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-23 01:31 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-23 01:31 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-23 01:31 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-23 01:31 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-23 01:31 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-23 01:31 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-23 01:31 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-23 01:31 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-23 01:31 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-23 01:31 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-23 01:31 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-23 01:31 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6058 b- defN 23-Jun-23 01:31 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-23 01:31 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2276 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4866 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    20939 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6763 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/kv_cache/position_embeddings_adjustment.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    10570 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-23 01:31 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-23 01:31 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-23 01:31 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-23 01:31 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-23 01:31 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-23 01:31 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-23 01:31 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-23 01:31 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-23 01:31 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-23 01:31 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-23 01:31 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-23 01:31 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-23 01:31 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-23 01:31 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-23 01:31 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-23 01:31 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-23 01:31 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-23 01:31 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-23 01:31 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-23 01:31 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-23 01:31 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-23 01:31 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-23 01:31 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-23 01:31 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-23 01:31 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-23 01:31 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-23 01:31 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-23 01:31 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-23 01:31 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-23 01:31 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-23 01:31 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-23 01:31 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-23 01:31 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-23 01:31 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-23 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-23 01:31 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-23 01:31 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-23 01:31 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-23 01:31 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-23 01:31 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-23 01:31 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-23 01:31 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-23 01:31 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-23 01:31 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     2190 b- defN 23-Jun-23 01:31 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6117 b- defN 23-Jun-23 01:31 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-23 01:31 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10884 b- defN 23-Jun-23 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-23 01:31 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-23 01:31 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-23 01:31 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20676 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-23 01:31 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-23 01:31 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-23 01:31 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-23 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-23 01:31 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-23 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-23 01:31 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-23 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-23 01:31 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-23 01:31 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-23 01:31 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-23 01:31 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-23 01:31 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-23 01:31 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-23 01:31 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-23 01:31 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-23 01:31 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-23 01:31 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-23 01:31 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-23 01:31 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-23 01:31 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    21290 b- defN 23-Jun-23 01:31 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-23 01:31 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-23 01:31 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-23 01:31 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-23 01:31 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-23 01:31 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-23 01:31 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-23 01:31 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-23 01:31 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-23 01:31 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-23 01:31 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-23 01:31 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-23 01:31 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-23 01:31 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-23 01:31 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-23 01:31 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-23 01:31 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-23 01:31 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-23 01:31 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-23 01:31 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-23 01:31 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-23 01:31 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-23 01:31 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-23 01:31 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-23 01:31 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-23 01:31 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-23 01:31 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-23 01:31 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    35086 b- defN 23-Jun-23 01:31 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-23 01:31 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-23 01:31 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-23 01:31 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-23 01:31 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-23 01:31 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21712 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37031 b- defN 23-Jun-23 01:33 sparseml_nightly-1.6.0.20230623.dist-info/RECORD
+372 files, 3472697 bytes uncompressed, 899562 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1089,29 +1089,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230616.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230623.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/onnx/optim/quantization/calibration.py

```diff
@@ -13,25 +13,27 @@
 # limitations under the License.
 
 """
 Provides a class for performing quantization calibration on an Onnx model.
 """
 
 
+import logging
 import os
-import tempfile
 from typing import Dict, Generator, Iterable, List, Tuple, Union
 
 import numpy as np
 import onnx
 
 from sparseml.onnx.utils import ORTModelRunner, fold_conv_bns, get_node_output_nodes
 from sparsezoo.utils import save_onnx, validate_onnx
 
 
+_LOGGER = logging.getLogger(__name__)
+
 __all__ = ["CalibrationSession"]
 
 
 class CalibrationSession:
     """
     Class for performing quantization calibration on an Onnx model.
 
@@ -61,19 +63,19 @@
         self._static = static
 
         self._model = onnx.load(self._onnx_file)
         self._optimized_model_path = self._optimize_model()
         self._model_augmented = self.generate_augmented_model()
 
         if self._augmented_model_path is None:
-            self._augmented_model_tmp_file = tempfile.NamedTemporaryFile(
-                suffix=".onnx", delete=True
+            self._augmented_model_path = os.path.join(
+                os.getcwd(), "model_augmented.onnx"
             )
-            self._augmented_model_path = self._augmented_model_tmp_file.name
         save_onnx(self._model_augmented, self._augmented_model_path)
+        _LOGGER.debug(f"Created an augmented model at: {self._augmented_model_path}")
 
         self._sessions = {}  # batch_size -> session
         self._quantization_thresholds = {}  # Dict[node.name, Tuple(min_val, max_val)]
 
     @property
     def model(self):
         """
@@ -99,21 +101,23 @@
         try:
             print("Optimizing {}...".format(self._onnx_file))
             model_optimized = fold_conv_bns(self._onnx_file)
             if model_optimized is None:
                 # no optimization performed, skip the rest of this block
                 raise Exception()
             validate_onnx(model_optimized)  # should raise exception if broken
-            optimized_model_path = tempfile.NamedTemporaryFile(
-                suffix=".onnx", delete=False
-            )
-            save_onnx(model_optimized, optimized_model_path.name)
+            optimized_model_path = os.path.join(os.getcwd(), "model_optimized.onnx")
+            save_onnx(model_optimized, optimized_model_path)
             self._model = model_optimized
-            print("Optimization successful")
-            return optimized_model_path.name
+            _LOGGER.debug(
+                "Optimization successful. "
+                "Created an optimized model at: "
+                f"{optimized_model_path}"
+            )
+            return optimized_model_path
         except Exception as e:
             print(e)
             print(
                 (
                     "WARNING: no conv-batch norms folded for {}, using original model"
                 ).format(self._onnx_file)
             )
@@ -348,7 +352,9 @@
 
     def __del__(self):
         """
         Cleans up any unnecessary files.
         """
         if self._optimized_model_path is not None:
             os.remove(self._optimized_model_path)
+        if self._augmented_model_path is not None:
+            os.remove(self._augmented_model_path)
```

## sparseml/pytorch/__init__.py

```diff
@@ -22,14 +22,25 @@
 from packaging import version
 
 
 try:
     import torch
 
     _PARSED_TORCH_VERSION = version.parse(torch.__version__)
+
+    if _PARSED_TORCH_VERSION.major >= 2:
+
+        torch_compile_func = torch.compile
+
+        def raise_torch_compile_warning(*args, **kwargs):
+            warnings.warn("torch.compile is not supported by sparseml for torch 2.0.x")
+            return torch_compile_func(*args, **kwargs)
+
+        torch.compile = raise_torch_compile_warning
+
     _BYPASS = bool(int(os.environ.get("NM_BYPASS_TORCH_VERSION", "0")))
     if _PARSED_TORCH_VERSION.major == 1 and _PARSED_TORCH_VERSION.minor in [10, 11]:
         if not _BYPASS:
             raise RuntimeError(
                 "sparseml does not support torch==1.10.* or 1.11.*. "
                 f"Found torch version {torch.__version__}.\n\n"
                 "To bypass this error, set environment variable "
```

## sparseml/pytorch/torch_to_onnx_exporter.py

```diff
@@ -10,15 +10,15 @@
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import collections
 import logging
-import tempfile
+import os
 import warnings
 from copy import deepcopy
 from typing import Any, Dict, Iterable, List
 
 import onnx
 import torch
 from packaging import version
@@ -143,17 +143,18 @@
         return model
 
     def post_validate(self, model: onnx.ModelProto) -> onnx.ModelProto:
         if not isinstance(model, onnx.ModelProto):
             raise TypeError(f"Expected onnx.ModelProto, found {type(model)}")
         return model
 
-    def transform(self, module: torch.nn.Module) -> onnx.ModelProto:
-        tmp = tempfile.NamedTemporaryFile("w")
-        file_path = tmp.name
+    def transform(
+        self, module: torch.nn.Module, file_name: str = "model.onnx"
+    ) -> onnx.ModelProto:
+        file_path = os.path.join(os.getcwd(), file_name)
 
         _LOGGER.debug(f"Saving onnx model to {file_path}")
 
         export_kwargs = deepcopy(self.export_kwargs)
 
         sample_batch = tensors_to_device(self.sample_batch, "cpu")
```

## sparseml/yolov8/trainers.py

```diff
@@ -276,14 +276,23 @@
             self.ema.updates = ckpt["updates"]
 
     def _setup_train(self, rank, world_size):
         super()._setup_train(rank, world_size)
         # NOTE: self.resume_training() was called in ^
 
         if rank in {0, -1}:
+            self.test_loader = self.get_dataloader(
+                self.testset,
+                batch_size=max(1, self.train_loader.batch_size // 4),
+                rank=-1,
+                mode="val",
+            )
+            self.validator = self.get_validator()
+
+        if rank in {0, -1}:
             config = dict(self.args)
             if self.manager is not None:
                 config["manager"] = str(self.manager)
             loggers = [PythonLogger(logger=LOGGER)]
             try:
                 init_kwargs = dict(config=config)
                 if self.args.project is not None:
```

## Comparing `sparseml_nightly-1.6.0.20230616.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230623.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230616.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230623.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230616
+Version: 1.6.0.20230623
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -29,15 +29,15 @@
 Requires-Dist: jupyter (>=1.0.0)
 Requires-Dist: ipywidgets (>=7.0.0)
 Requires-Dist: pyyaml (>=5.0.0)
 Requires-Dist: progressbar2 (>=3.0.0)
 Requires-Dist: numpy (<=1.21.6,>=1.0.0)
 Requires-Dist: matplotlib (>=3.0.0)
 Requires-Dist: merge-args (>=0.1.0)
-Requires-Dist: onnx (<=1.12.0,>=1.5.0)
+Requires-Dist: onnx (<1.15.0,>=1.5.0)
 Requires-Dist: pandas (>=0.25.0)
 Requires-Dist: packaging (>=20.0)
 Requires-Dist: psutil (>=5.0.0)
 Requires-Dist: pydantic (>=1.5.0)
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: scikit-image (>=0.15.0)
 Requires-Dist: scikit-learn (>=0.24.2)
@@ -106,14 +106,15 @@
 Provides-Extra: transformers
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'transformers'
 Requires-Dist: gputils ; extra == 'transformers'
 Requires-Dist: nm-transformers-nightly (~=1.6.0) ; extra == 'transformers'
 Requires-Dist: datasets (<=1.18.4) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
+Requires-Dist: accelerate (>=0.20.3) ; extra == 'transformers'
 Provides-Extra: ultralytics
 Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'ultralytics'
 Provides-Extra: yolov5
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
 Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'yolov5'
```

## Comparing `sparseml_nightly-1.6.0.20230616.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230623.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230616.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230623.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 sparseml/onnx/framework/__init__.py,sha256=HpgplVizgXIPOmnE24RM1geQLp924227_T12jJjQCaA,823
 sparseml/onnx/framework/info.py,sha256=YzZmDaR6Z1y66xo_OKtmQGA1ZVFOozZNXBJ_Ec74ueU,6116
 sparseml/onnx/optim/__init__.py,sha256=EZeHGH5zDRfb0MrXqh4_3ci0ViBS2WWb8NqhAi8nd3A,820
 sparseml/onnx/optim/analyzer_model.py,sha256=6nfKmLzdwesxupN_PWNLCGtXPk2uf4L5OOBBuzSNvQ4,13285
 sparseml/onnx/optim/sensitivity_pruning.py,sha256=L-Sp669RNH4BaZJ3JTcDvcoaOZEE1URFxALPVq3z9rY,19639
 sparseml/onnx/optim/structured_pruning.py,sha256=XyyoNqa7855JM-R3B6UgSez2h4V1EuEi4jUhuK0ztT8,6470
 sparseml/onnx/optim/quantization/__init__.py,sha256=mKe75Yza1RlQOe43pcLb-IzWJD34LhwAALF7LYU2f2E,815
-sparseml/onnx/optim/quantization/calibration.py,sha256=cVcUyv4aXiTBeUMM7PSl7Ta7OJICVS63WJB2jBqWJFM,14532
+sparseml/onnx/optim/quantization/calibration.py,sha256=j4fArYgCxN1S6ign8QPKV1OS9eV3fvWn5rmeaq72g9o,14753
 sparseml/onnx/optim/quantization/quantize.py,sha256=TXrlfpE3NssIJuAzdDctWG3w9jCF82PXJDC46GRMJLA,73551
 sparseml/onnx/optim/quantization/quantize_model_post_training.py,sha256=aoz5ixUpQB_6XkowhozqRp8_njthBeqVuwvV2ctM1q0,4552
 sparseml/onnx/sparsification/__init__.py,sha256=hFZDQQXFcXqSqiXlRBRUX7e7GavLphgRd8c21peq8fg,869
 sparseml/onnx/sparsification/analyzer.py,sha256=DCKc8nYo0i3NDu73GVjvBYjuflXUZhkhB14FoFRlTBE,10209
 sparseml/onnx/sparsification/info.py,sha256=UnrwVgOuj-HErwTMc-19h-QOrs1yG_mM45O9VL8oiXU,1363
 sparseml/onnx/sparsification/model_info.py,sha256=Y0tpY9fWN3gr4KlkAdXv2QYJrrrjMvVZOCA-ujPJFPM,8009
 sparseml/onnx/utils/__init__.py,sha256=fGZED95Xmko70ZmTWlZWX3-C4dajmbZcKgaap3HXmVw,867
@@ -118,18 +118,18 @@
 sparseml/openpifpaf/trainer.py,sha256=Du9W5fW9ImC3XlOVVWesbcBv1SjJOfP_D94_hBUR6VY,4211
 sparseml/optim/__init__.py,sha256=3oGQ4LY0MSrbTAwuyPHEOEyYiZ7JI7OX2BgWup5NPuw,882
 sparseml/optim/analyzer.py,sha256=LUYBYyvfVwaw_V1aAiOmaybUGJQk4vRK5RG3k3nD7pA,6302
 sparseml/optim/helpers.py,sha256=Zb7YPYe07vuVyYUhHJ-BlcMrZa-sxt1TUZ-Ec9Z6o_U,25563
 sparseml/optim/manager.py,sha256=KeDVHj9ea9EUaV908qfvq8ONwS8nUmAvQb1yXflOBWo,25984
 sparseml/optim/modifier.py,sha256=qYfVUL9thw94p4oEsNZgitUJ3y9izWYb8nUI3enyzOU,30708
 sparseml/optim/sensitivity.py,sha256=neMP_hTRqzDUV0MrATevC2-JQYnOIvNW_AlIf_y_ydw,26315
-sparseml/pytorch/__init__.py,sha256=3E40C1X1fjhlU0ZwdHZ-xhORHb-qDUtr7ALDv9xbzI0,1848
+sparseml/pytorch/__init__.py,sha256=n1a6y27bzfG73uLbifhIx5DY9hDg1RM1pTIN1DgBpDw,2190
 sparseml/pytorch/base.py,sha256=C5ced9i5Y_fy-cnYkEFt6GuOGDHYu7fZ3pHrCm1W6mE,6117
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
-sparseml/pytorch/torch_to_onnx_exporter.py,sha256=78Ft0yuGVKx3TMhPeG9e3o6dI2GC_432VwuiKokfZuc,10864
+sparseml/pytorch/torch_to_onnx_exporter.py,sha256=HHgmXDopADURZcO50F5pX2wNffQGykWkwy0aTYw2H0U,10884
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
 sparseml/pytorch/datasets/registry.py,sha256=cEA3d5ju5EMft92f2StVLWARnAxlRpidKZaozujmFdE,2814
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
 sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
 sparseml/pytorch/datasets/classification/imagefolder.py,sha256=rOvwqy2Zp89VkT7zat2hQxRmgPyvCpSAhZ4mWEsL9JI,3669
 sparseml/pytorch/datasets/classification/imagenet.py,sha256=CHzsckzsSsUCLR-oxaxJ8NH7j4WBqg_Wg5ge27bPk5Q,4000
@@ -353,20 +353,20 @@
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=mzOuog5BmQg3tER3m35zqTcKRlxiw9IqCpgBy-Ep1sA,34788
+sparseml/yolov8/trainers.py,sha256=AAMOpH47N-T4RmNENWbXMW-nkmaXKamwtVNXQtudtCM,35086
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230616.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230616.dist-info/METADATA,sha256=mbldDmE0rs01lQ8U9i7yYQQ1bq_cVkmu72tEVdd2lyo,21650
-sparseml_nightly-1.6.0.20230616.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230616.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230616.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
-sparseml_nightly-1.6.0.20230616.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230616.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230623.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230623.dist-info/METADATA,sha256=mKbU7V6spYb5nC2DAr2dmqu54dKylG_nxSEFuH1CWkQ,21712
+sparseml_nightly-1.6.0.20230623.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230623.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230623.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
+sparseml_nightly-1.6.0.20230623.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230623.dist-info/RECORD,,
```

