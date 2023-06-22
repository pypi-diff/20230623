# Comparing `tmp/xGPR-0.1.2.1.tar.gz` & `tmp/xGPR-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xGPR-0.1.2.1.tar", last modified: Wed Jun 21 00:05:12 2023, max compression
+gzip compressed data, was "xGPR-0.1.2.2.tar", last modified: Thu Jun 22 23:18:15 2023, max compression
```

## Comparing `xGPR-0.1.2.1.tar` & `xGPR-0.1.2.2.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/LICENSE
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/README.md
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       78 2023-06-21 00:02:39.000000 xGPR-0.1.2.1/pyproject.toml
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/setup.cfg
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.2.1/setup.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.796276 xGPR-0.1.2.1/xGPR/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-21 00:04:56.000000 xGPR-0.1.2.1/xGPR/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.796276 xGPR-0.1.2.1/xGPR/cg_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/cg_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/cg_toolkit/cg_linear_operators.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/cg_toolkit/cg_tools.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/cg_toolkit/cuda_cg_linear_operators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.796276 xGPR-0.1.2.1/xGPR/constants/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/constants/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.2.1/xGPR/constants/constants.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.796276 xGPR-0.1.2.1/xGPR/data_handling/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/data_handling/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/data_handling/data_handling_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13221 2023-06-07 22:51:35.000000 xGPR-0.1.2.1/xGPR/data_handling/dataset_builder.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/data_handling/minibatch_data_handler.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/data_handling/offline_data_handling.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.2.1/xGPR/data_handling/online_data_handling.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.796276 xGPR-0.1.2.1/xGPR/fitting_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/fitting_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.2.1/xGPR/fitting_toolkit/ams_grad_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.2.1/xGPR/fitting_toolkit/cg_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.2.1/xGPR/fitting_toolkit/exact_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.2.1/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.2.1/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/kernels/
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/kernels/ARD_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.2.1/xGPR/kernels/ARD_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13201 2023-06-19 15:11:57.000000 xGPR-0.1.2.1/xGPR/kernels/ARD_kernels/mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-06-16 16:46:38.000000 xGPR-0.1.2.1/xGPR/kernels/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3507 2023-06-19 13:59:18.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3206 2023-06-19 14:13:44.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/matern.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7009 2023-06-19 14:10:03.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/polynomial.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1951 2023-06-19 14:14:22.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11293 2023-06-19 15:12:56.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8197 2023-06-19 15:13:21.000000 xGPR-0.1.2.1/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8097 2023-06-17 22:46:55.000000 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10417 2023-06-19 15:13:46.000000 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/fht_conv1d.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-06-19 15:14:09.000000 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/graph_arccos.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7287 2023-06-19 15:14:30.000000 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/graph_polysum.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7806 2023-06-19 15:16:23.000000 xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/graph_rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15507 2023-06-19 13:53:19.000000 xGPR-0.1.2.1/xGPR/kernels/kernel_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.2.1/xGPR/kernels/srht_compressor.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/optimizers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/optimizers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/optimizers/bayes_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/optimizers/crude_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/optimizers/lb_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/optimizers/map_loss_bayes_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/optimizers/pure_bayes_optimizer.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/preconditioners/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/preconditioners/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.2.1/xGPR/preconditioners/inter_device_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/preconditioners/rand_nys_constructors.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/preconditioners/rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/preconditioners/tuning_preconditioners.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/random_feature_generation/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21805 2023-06-20 23:27:23.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12508 2023-06-19 14:41:23.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15398 2023-06-20 23:28:13.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.800277 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23784 2023-06-20 23:29:00.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15776 2023-06-20 23:30:00.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
--rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27786 2023-06-19 23:39:23.000000 xGPR-0.1.2.1/xGPR/regression_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/scoring_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/scoring_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/scoring_toolkit/approximate_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/scoring_toolkit/cho_solvers.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5907 2023-06-20 17:26:24.000000 xGPR-0.1.2.1/xGPR/scoring_toolkit/exact_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/scoring_toolkit/nmll_gradient_tools.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.2.1/xGPR/scoring_toolkit/probe_generators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/static_layers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/static_layers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9524 2023-06-17 22:48:21.000000 xGPR-0.1.2.1/xGPR/static_layers/fast_conv.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/tuning_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/tuning_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/tuning_toolkit/direct_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/tuning_toolkit/hparam_scoring.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.804277 xGPR-0.1.2.1/xGPR/visualization_tools/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.2.1/xGPR/visualization_tools/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.2.1/xGPR/visualization_tools/kernel_xpca.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-16 17:55:48.000000 xGPR-0.1.2.1/xGPR/xGP_Regression.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-21 00:05:12.796276 xGPR-0.1.2.1/xGPR.egg-info/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-21 00:05:12.000000 xGPR-0.1.2.1/xGPR.egg-info/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6971 2023-06-21 00:05:12.000000 xGPR-0.1.2.1/xGPR.egg-info/SOURCES.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-21 00:05:12.000000 xGPR-0.1.2.1/xGPR.egg-info/dependency_links.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-21 00:05:12.000000 xGPR-0.1.2.1/xGPR.egg-info/requires.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-21 00:05:12.000000 xGPR-0.1.2.1/xGPR.egg-info/top_level.txt
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.091404 xGPR-0.1.2.2/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/LICENSE
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-22 23:18:15.091404 xGPR-0.1.2.2/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/README.md
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       78 2023-06-21 00:02:39.000000 xGPR-0.1.2.2/pyproject.toml
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-22 23:18:15.091404 xGPR-0.1.2.2/setup.cfg
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.2.2/setup.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.651403 xGPR-0.1.2.2/xGPR/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-22 23:05:17.000000 xGPR-0.1.2.2/xGPR/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.711403 xGPR-0.1.2.2/xGPR/cg_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/cg_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/cg_toolkit/cg_linear_operators.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/cg_toolkit/cg_tools.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/cg_toolkit/cuda_cg_linear_operators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.711403 xGPR-0.1.2.2/xGPR/constants/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/constants/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.2.2/xGPR/constants/constants.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.727403 xGPR-0.1.2.2/xGPR/data_handling/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/data_handling/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/data_handling/data_handling_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13191 2023-06-22 23:01:08.000000 xGPR-0.1.2.2/xGPR/data_handling/dataset_builder.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/data_handling/minibatch_data_handler.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/data_handling/offline_data_handling.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.2.2/xGPR/data_handling/online_data_handling.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.779403 xGPR-0.1.2.2/xGPR/fitting_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/fitting_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.2.2/xGPR/fitting_toolkit/ams_grad_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.2.2/xGPR/fitting_toolkit/cg_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.2.2/xGPR/fitting_toolkit/exact_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.2.2/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.2.2/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.831403 xGPR-0.1.2.2/xGPR/kernels/
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.851404 xGPR-0.1.2.2/xGPR/kernels/ARD_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.2.2/xGPR/kernels/ARD_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13201 2023-06-19 15:11:57.000000 xGPR-0.1.2.2/xGPR/kernels/ARD_kernels/mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-06-16 16:46:38.000000 xGPR-0.1.2.2/xGPR/kernels/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.915404 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3507 2023-06-19 13:59:18.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3206 2023-06-19 14:13:44.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/matern.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7009 2023-06-19 14:10:03.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/polynomial.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1951 2023-06-19 14:14:22.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11293 2023-06-19 15:12:56.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/rbf_linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8197 2023-06-19 15:13:21.000000 xGPR-0.1.2.2/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.959404 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8097 2023-06-17 22:46:55.000000 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10417 2023-06-19 15:13:46.000000 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/fht_conv1d.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-06-19 15:14:09.000000 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/graph_arccos.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7287 2023-06-19 15:14:30.000000 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/graph_polysum.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7806 2023-06-19 15:16:23.000000 xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/graph_rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15507 2023-06-19 13:53:19.000000 xGPR-0.1.2.2/xGPR/kernels/kernel_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.2.2/xGPR/kernels/srht_compressor.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.015404 xGPR-0.1.2.2/xGPR/optimizers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/optimizers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/optimizers/bayes_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/optimizers/crude_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/optimizers/lb_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/optimizers/map_loss_bayes_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/optimizers/pure_bayes_optimizer.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.035404 xGPR-0.1.2.2/xGPR/preconditioners/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/preconditioners/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.2.2/xGPR/preconditioners/inter_device_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/preconditioners/rand_nys_constructors.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/preconditioners/rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/preconditioners/tuning_preconditioners.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.039404 xGPR-0.1.2.2/xGPR/random_feature_generation/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.039404 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.039404 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.043404 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21805 2023-06-20 23:27:23.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12508 2023-06-19 14:41:23.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15398 2023-06-20 23:28:13.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.043404 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.043404 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.047404 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.047404 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.051404 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23784 2023-06-20 23:29:00.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15776 2023-06-20 23:30:00.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
+-rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.051404 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    27786 2023-06-19 23:39:23.000000 xGPR-0.1.2.2/xGPR/regression_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.071404 xGPR-0.1.2.2/xGPR/scoring_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/scoring_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/scoring_toolkit/approximate_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/scoring_toolkit/cho_solvers.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5907 2023-06-20 17:26:24.000000 xGPR-0.1.2.2/xGPR/scoring_toolkit/exact_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/scoring_toolkit/nmll_gradient_tools.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.2.2/xGPR/scoring_toolkit/probe_generators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.071404 xGPR-0.1.2.2/xGPR/static_layers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/static_layers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9524 2023-06-17 22:48:21.000000 xGPR-0.1.2.2/xGPR/static_layers/fast_conv.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.087404 xGPR-0.1.2.2/xGPR/tuning_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/tuning_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/tuning_toolkit/direct_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/tuning_toolkit/hparam_scoring.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:15.091404 xGPR-0.1.2.2/xGPR/visualization_tools/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.2.2/xGPR/visualization_tools/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.2.2/xGPR/visualization_tools/kernel_xpca.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-16 17:55:48.000000 xGPR-0.1.2.2/xGPR/xGP_Regression.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-22 23:18:14.675403 xGPR-0.1.2.2/xGPR.egg-info/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-22 23:18:14.000000 xGPR-0.1.2.2/xGPR.egg-info/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6971 2023-06-22 23:18:14.000000 xGPR-0.1.2.2/xGPR.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-22 23:18:14.000000 xGPR-0.1.2.2/xGPR.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-22 23:18:14.000000 xGPR-0.1.2.2/xGPR.egg-info/requires.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-22 23:18:14.000000 xGPR-0.1.2.2/xGPR.egg-info/top_level.txt
```

### Comparing `xGPR-0.1.2.1/LICENSE` & `xGPR-0.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/PKG-INFO` & `xGPR-0.1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.2.1/README.md` & `xGPR-0.1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/setup.py` & `xGPR-0.1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/cg_toolkit/cg_linear_operators.py` & `xGPR-0.1.2.2/xGPR/cg_toolkit/cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/cg_toolkit/cg_tools.pyx` & `xGPR-0.1.2.2/xGPR/cg_toolkit/cg_tools.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/cg_toolkit/cuda_cg_linear_operators.py` & `xGPR-0.1.2.2/xGPR/cg_toolkit/cuda_cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/constants/constants.py` & `xGPR-0.1.2.2/xGPR/constants/constants.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/data_handling/data_handling_baseclass.py` & `xGPR-0.1.2.2/xGPR/data_handling/data_handling_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/data_handling/dataset_builder.py` & `xGPR-0.1.2.2/xGPR/data_handling/dataset_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             if len(x_data.shape) != 3:
                 raise ValueError(f"File {xfile} is not a 3d array, but you have called "
                 "build_offline_3d_dataset.")
 
             if xdim[1] == -1:
                 xdim[1] = x_data.shape[1]
                 xdim[2] = x_data.shape[2]
-            elif x_data.shape[1] != xdim[1] or x_data.shape[2] != xdim[2]:
+            elif x_data.shape[2] != xdim[2]:
                 raise ValueError("All x arrays must have the same dimensionality.")
             if x_data.shape[0] > chunk_size:
                 raise ValueError(f"Xfile {xfile} has more datapoints than allowed "
                     "based on specified chunk_size. Either increase chunk_size "
                     "or divide your data into np.ndarrays saved on disk that each "
                     "contain < chunk_size datapoints.")
             if len(yshape) > 1:
```

### Comparing `xGPR-0.1.2.1/xGPR/data_handling/minibatch_data_handler.py` & `xGPR-0.1.2.2/xGPR/data_handling/minibatch_data_handler.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/data_handling/offline_data_handling.py` & `xGPR-0.1.2.2/xGPR/data_handling/offline_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/data_handling/online_data_handling.py` & `xGPR-0.1.2.2/xGPR/data_handling/online_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/fitting_toolkit/ams_grad_toolkit.py` & `xGPR-0.1.2.2/xGPR/fitting_toolkit/ams_grad_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/fitting_toolkit/cg_fitting_toolkit.py` & `xGPR-0.1.2.2/xGPR/fitting_toolkit/cg_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/fitting_toolkit/exact_fitting_toolkit.py` & `xGPR-0.1.2.2/xGPR/fitting_toolkit/exact_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py` & `xGPR-0.1.2.2/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/fitting_toolkit/sgd_fitting_toolkit.py` & `xGPR-0.1.2.2/xGPR/fitting_toolkit/sgd_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/ARD_kernels/mini_ard.py` & `xGPR-0.1.2.2/xGPR/kernels/ARD_kernels/mini_ard.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/__init__.py` & `xGPR-0.1.2.2/xGPR/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/basic_kernels/linear.py` & `xGPR-0.1.2.2/xGPR/kernels/basic_kernels/linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/basic_kernels/matern.py` & `xGPR-0.1.2.2/xGPR/kernels/basic_kernels/matern.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/basic_kernels/polynomial.py` & `xGPR-0.1.2.2/xGPR/kernels/basic_kernels/polynomial.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/basic_kernels/rbf.py` & `xGPR-0.1.2.2/xGPR/kernels/basic_kernels/rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/basic_kernels/rbf_linear.py` & `xGPR-0.1.2.2/xGPR/kernels/basic_kernels/rbf_linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py` & `xGPR-0.1.2.2/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/conv_feature_extractor.py` & `xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/conv_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/fht_conv1d.py` & `xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/fht_conv1d.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/graph_arccos.py` & `xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/graph_arccos.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/graph_polysum.py` & `xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/graph_polysum.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/convolution_kernels/graph_rbf.py` & `xGPR-0.1.2.2/xGPR/kernels/convolution_kernels/graph_rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/kernel_baseclass.py` & `xGPR-0.1.2.2/xGPR/kernels/kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/kernels/srht_compressor.py` & `xGPR-0.1.2.2/xGPR/kernels/srht_compressor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/optimizers/bayes_grid_optimizer.py` & `xGPR-0.1.2.2/xGPR/optimizers/bayes_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/optimizers/crude_grid_optimizer.py` & `xGPR-0.1.2.2/xGPR/optimizers/crude_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/optimizers/lb_optimizer.py` & `xGPR-0.1.2.2/xGPR/optimizers/lb_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/optimizers/map_loss_bayes_optimizer.py` & `xGPR-0.1.2.2/xGPR/optimizers/map_loss_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/optimizers/pure_bayes_optimizer.py` & `xGPR-0.1.2.2/xGPR/optimizers/pure_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/preconditioners/cuda_rand_nys_preconditioners.py` & `xGPR-0.1.2.2/xGPR/preconditioners/cuda_rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/preconditioners/inter_device_preconditioners.py` & `xGPR-0.1.2.2/xGPR/preconditioners/inter_device_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/preconditioners/rand_nys_constructors.py` & `xGPR-0.1.2.2/xGPR/preconditioners/rand_nys_constructors.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/preconditioners/rand_nys_preconditioners.py` & `xGPR-0.1.2.2/xGPR/preconditioners/rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/preconditioners/tuning_preconditioners.py` & `xGPR-0.1.2.2/xGPR/preconditioners/tuning_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.2.2/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/regression_baseclass.py` & `xGPR-0.1.2.2/xGPR/regression_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/scoring_toolkit/approximate_nmll_calcs.py` & `xGPR-0.1.2.2/xGPR/scoring_toolkit/approximate_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/scoring_toolkit/cho_solvers.py` & `xGPR-0.1.2.2/xGPR/scoring_toolkit/cho_solvers.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/scoring_toolkit/exact_nmll_calcs.py` & `xGPR-0.1.2.2/xGPR/scoring_toolkit/exact_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/scoring_toolkit/nmll_gradient_tools.py` & `xGPR-0.1.2.2/xGPR/scoring_toolkit/nmll_gradient_tools.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/scoring_toolkit/probe_generators.py` & `xGPR-0.1.2.2/xGPR/scoring_toolkit/probe_generators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/static_layers/fast_conv.py` & `xGPR-0.1.2.2/xGPR/static_layers/fast_conv.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py` & `xGPR-0.1.2.2/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/tuning_toolkit/direct_fitting_optimizer.py` & `xGPR-0.1.2.2/xGPR/tuning_toolkit/direct_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/tuning_toolkit/hparam_scoring.py` & `xGPR-0.1.2.2/xGPR/tuning_toolkit/hparam_scoring.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/visualization_tools/kernel_xpca.py` & `xGPR-0.1.2.2/xGPR/visualization_tools/kernel_xpca.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR/xGP_Regression.py` & `xGPR-0.1.2.2/xGPR/xGP_Regression.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.1/xGPR.egg-info/PKG-INFO` & `xGPR-0.1.2.2/xGPR.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.2.1/xGPR.egg-info/SOURCES.txt` & `xGPR-0.1.2.2/xGPR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

