# Comparing `tmp/ANNarchy-4.7.2.3.tar.gz` & `tmp/ANNarchy-4.7.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANNarchy-4.7.2.3.tar", last modified: Thu May 25 07:32:25 2023, max compression
+gzip compressed data, was "ANNarchy-4.7.2.4.tar", last modified: Fri Jun 23 04:26:37 2023, max compression
```

## Comparing `ANNarchy-4.7.2.3.tar` & `ANNarchy-4.7.2.4.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.868828 ANNarchy-4.7.2.3/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.819674 ANNarchy-4.7.2.3/ANNarchy/
--rw-r--r--   0 vitay      (501) staff       (20)     1989 2023-05-25 07:29:05.000000 ANNarchy-4.7.2.3/ANNarchy/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.825003 ANNarchy-4.7.2.3/ANNarchy/core/
--rw-r--r--   0 vitay      (501) staff       (20)    27962 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/ConnectorMethods.py
--rw-r--r--   0 vitay      (501) staff       (20)    13851 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Dendrite.py
--rw-r--r--   0 vitay      (501) staff       (20)    28338 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Global.py
--rw-r--r--   0 vitay      (501) staff       (20)    19614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/IO.py
--rw-r--r--   0 vitay      (501) staff       (20)    35087 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/Monitor.py
--rw-r--r--   0 vitay      (501) staff       (20)    34361 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/Network.py
--rw-r--r--   0 vitay      (501) staff       (20)     7309 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/NetworkManager.py
--rw-r--r--   0 vitay      (501) staff       (20)     8453 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/Neuron.py
--rw-r--r--   0 vitay      (501) staff       (20)    32634 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Population.py
--rw-r--r--   0 vitay      (501) staff       (20)    12829 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/PopulationView.py
--rw-r--r--   0 vitay      (501) staff       (20)     6876 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/Profiler.py
--rw-r--r--   0 vitay      (501) staff       (20)    65222 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/core/Projection.py
--rw-r--r--   0 vitay      (501) staff       (20)     8383 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/ANNarchy/core/Random.py
--rw-r--r--   0 vitay      (501) staff       (20)    10098 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/Simulate.py
--rw-r--r--   0 vitay      (501) staff       (20)    95403 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/SpecificPopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)    15140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/core/SpecificProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)     5803 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/Synapse.py
--rw-r--r--   0 vitay      (501) staff       (20)     3463 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)        1 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/core/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.825823 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/
--rw-r--r--   0 vitay      (501) staff       (20)     1683 2022-05-18 09:30:59.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pxd
--rw-r--r--   0 vitay      (501) staff       (20)    21582 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pyx
--rw-r--r--   0 vitay      (501) staff       (20)      924 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pxd
--rw-r--r--   0 vitay      (501) staff       (20)     4941 2022-01-07 10:51:43.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pyx
--rw-r--r--   0 vitay      (501) staff       (20)     2866 2022-02-02 12:38:23.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Transformations.pyx
--rw-r--r--   0 vitay      (501) staff       (20)        0 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/__init__.pxd
--rw-r--r--   0 vitay      (501) staff       (20)      405 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.826001 ANNarchy-4.7.2.3/ANNarchy/extensions/
--rw-r--r--   0 vitay      (501) staff       (20)       21 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.826455 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/
--rw-r--r--   0 vitay      (501) staff       (20)     9131 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
--rw-r--r--   0 vitay      (501) staff       (20)     3621 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
--rw-r--r--   0 vitay      (501) staff       (20)       48 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.827787 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/
--rw-r--r--   0 vitay      (501) staff       (20)    12839 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/AccProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)     2928 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldModel.py
--rw-r--r--   0 vitay      (501) staff       (20)    10439 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldMonitor.py
--rw-r--r--   0 vitay      (501) staff       (20)    15160 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/NormProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)    27888 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/PredefinedModels.py
--rw-r--r--   0 vitay      (501) staff       (20)      386 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/bold/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.829730 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/
--rw-r--r--   0 vitay      (501) staff       (20)    42897 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Convolve.py
--rw-r--r--   0 vitay      (501) staff       (20)     3005 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/ConvolveTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     9368 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Copy.py
--rw-r--r--   0 vitay      (501) staff       (20)     4502 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/CopyTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    24982 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Pooling.py
--rw-r--r--   0 vitay      (501) staff       (20)    14070 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/PoolingTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    14093 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Transpose.py
--rw-r--r--   0 vitay      (501) staff       (20)     1583 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)      858 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.830069 ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/
--rw-r--r--   0 vitay      (501) staff       (20)    16351 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/DiagonalProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)       50 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.830458 ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/
--rw-r--r--   0 vitay      (501) staff       (20)    20781 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/HybridPopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       72 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.830909 ANNarchy-4.7.2.3/ANNarchy/extensions/image/
--rw-r--r--   0 vitay      (501) staff       (20)     9944 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/image/ImagePopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       62 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/image/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.831357 ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/
--rw-r--r--   0 vitay      (501) staff       (20)    12742 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/Logger.py
--rw-r--r--   0 vitay      (501) staff       (20)       26 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.832106 ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/
--rw-r--r--   0 vitay      (501) staff       (20)    51579 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/SharedProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)      206 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.834235 ANNarchy-4.7.2.3/ANNarchy/generator/
--rw-r--r--   0 vitay      (501) staff       (20)    42289 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/CodeGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    38169 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Compiler.py
--rw-r--r--   0 vitay      (501) staff       (20)    10654 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/MonitorGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.835903 ANNarchy-4.7.2.3/ANNarchy/generator/Population/
--rw-r--r--   0 vitay      (501) staff       (20)    59484 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDAGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    26498 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDATemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    41946 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    14427 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    20938 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/PopulationGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    37140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    13356 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)      142 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Population/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.836799 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/
--rw-r--r--   0 vitay      (501) staff       (20)    14883 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CPP11Profile.py
--rw-r--r--   0 vitay      (501) staff       (20)     8646 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CUDAProfile.py
--rw-r--r--   0 vitay      (501) staff       (20)     6963 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/PAPIProfile.py
--rw-r--r--   0 vitay      (501) staff       (20)     3947 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    31714 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)      159 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Profile/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.838911 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.841756 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/
--rw-r--r--   0 vitay      (501) staff       (20)    14633 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    11089 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    11052 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    36964 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    13010 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
--rw-r--r--   0 vitay      (501) staff       (20)    12651 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    15654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
--rw-r--r--   0 vitay      (501) staff       (20)    19628 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)    11220 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    15997 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)    15664 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)     8341 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/HYB.py
--rw-r--r--   0 vitay      (501) staff       (20)    10511 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1514 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    72468 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDAGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.844078 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/
--rw-r--r--   0 vitay      (501) staff       (20)     8715 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    13744 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)     3654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    37572 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)     8436 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py
--rw-r--r--   0 vitay      (501) staff       (20)     8172 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     6031 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
--rw-r--r--   0 vitay      (501) staff       (20)    19185 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)     4756 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     8759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     5111 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)    51527 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL.py
--rw-r--r--   0 vitay      (501) staff       (20)    22149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py
--rw-r--r--   0 vitay      (501) staff       (20)     4136 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1565 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    60579 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMPGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    49850 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/ProjectionGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.847124 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/
--rw-r--r--   0 vitay      (501) staff       (20)     8717 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    11194 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)     3413 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    37503 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)     7292 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    17125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)     4489 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
--rw-r--r--   0 vitay      (501) staff       (20)     4792 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     4570 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     8588 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)    14808 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)     4607 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/HYB.py
--rw-r--r--   0 vitay      (501) staff       (20)    45456 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/LIL.py
--rw-r--r--   0 vitay      (501) staff       (20)     4120 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1671 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    57963 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThreadGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)      233 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Projection/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    54049 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/PyxGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    15018 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Sanity.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.848614 ANNarchy-4.7.2.3/ANNarchy/generator/Template/
--rw-r--r--   0 vitay      (501) staff       (20)    29830 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/BaseTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    16113 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/GlobalOperationTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     2426 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/MakefileTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    19390 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/MonitorTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    14699 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/PyxTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)        0 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Template/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    15650 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/generator/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)       30 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.3/ANNarchy/generator/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.853227 ANNarchy-4.7.2.3/ANNarchy/include/
--rw-r--r--   0 vitay      (501) staff       (20)    26125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     6674 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    17338 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/COOMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8165 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/COOMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9119 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8274 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     7660 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDAT.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    22237 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixT.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    21843 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8971 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    30517 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8778 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    10925 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixOffsets.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    32735 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9264 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    30967 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    10305 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    19241 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     5284 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9991 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/LILInvMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    37614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/LILMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    23769 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/PartitionedMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    25554 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9628 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     1092 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/Specific.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     1430 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/ANNarchy/include/helper_functions.hpp
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.854385 ANNarchy-4.7.2.3/ANNarchy/models/
--rw-r--r--   0 vitay      (501) staff       (20)    45126 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/models/Neurons.py
--rw-r--r--   0 vitay      (501) staff       (20)    11837 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/models/Synapses.py
--rw-r--r--   0 vitay      (501) staff       (20)      352 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/models/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.857325 ANNarchy-4.7.2.3/ANNarchy/parser/
--rw-r--r--   0 vitay      (501) staff       (20)    15017 2023-05-24 12:05:12.000000 ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseNeuron.py
--rw-r--r--   0 vitay      (501) staff       (20)    21586 2023-05-24 12:08:11.000000 ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseSynapse.py
--rw-r--r--   0 vitay      (501) staff       (20)    14166 2023-05-24 12:05:32.000000 ANNarchy-4.7.2.3/ANNarchy/parser/CoupledEquations.py
--rw-r--r--   0 vitay      (501) staff       (20)    28868 2023-05-24 12:05:45.000000 ANNarchy-4.7.2.3/ANNarchy/parser/Equation.py
--rw-r--r--   0 vitay      (501) staff       (20)    28842 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/parser/Extraction.py
--rw-r--r--   0 vitay      (501) staff       (20)     4336 2022-12-05 16:13:02.000000 ANNarchy-4.7.2.3/ANNarchy/parser/Function.py
--rw-r--r--   0 vitay      (501) staff       (20)     6049 2022-12-05 16:13:18.000000 ANNarchy-4.7.2.3/ANNarchy/parser/ITE.py
--rw-r--r--   0 vitay      (501) staff       (20)     3032 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/ANNarchy/parser/ParserTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     7633 2022-12-05 16:13:32.000000 ANNarchy-4.7.2.3/ANNarchy/parser/StringManipulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       86 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/parser/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.858782 ANNarchy-4.7.2.3/ANNarchy/parser/report/
--rw-r--r--   0 vitay      (501) staff       (20)    16861 2023-01-25 15:17:04.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexParser.py
--rw-r--r--   0 vitay      (501) staff       (20)    22678 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexReport.py
--rw-r--r--   0 vitay      (501) staff       (20)    15846 2021-04-01 06:34:12.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/MarkdownReport.py
--rw-r--r--   0 vitay      (501) staff       (20)     1985 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/Report.py
--rw-r--r--   0 vitay      (501) staff       (20)        0 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/ANNarchy/parser/report/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.858864 ANNarchy-4.7.2.3/ANNarchy/thirdparty/
--rw-r--r--   0 vitay      (501) staff       (20)    26759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/ANNarchy/thirdparty/randutils.hpp
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.820472 ANNarchy-4.7.2.3/ANNarchy.egg-info/
--rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/PKG-INFO
--rw-r--r--   0 vitay      (501) staff       (20)     8626 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/SOURCES.txt
--rw-r--r--   0 vitay      (501) staff       (20)        1 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/dependency_links.txt
--rw-r--r--   0 vitay      (501) staff       (20)        1 2021-04-13 07:32:27.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/not-zip-safe
--rw-r--r--   0 vitay      (501) staff       (20)       36 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/requires.txt
--rw-r--r--   0 vitay      (501) staff       (20)        9 2023-05-25 07:32:25.000000 ANNarchy-4.7.2.3/ANNarchy.egg-info/top_level.txt
--rw-r--r--   0 vitay      (501) staff       (20)    18092 2017-07-25 21:20:59.000000 ANNarchy-4.7.2.3/LICENSE
--rw-r--r--   0 vitay      (501) staff       (20)      274 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.3/MANIFEST.in
--rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-05-25 07:32:25.868924 ANNarchy-4.7.2.3/PKG-INFO
--rw-r--r--   0 vitay      (501) staff       (20)     1803 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/README.md
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.818329 ANNarchy-4.7.2.3/examples/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.859231 ANNarchy-4.7.2.3/examples/ann_to_snn/
--rw-r--r--   0 vitay      (501) staff       (20)      991 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/examples/ann_to_snn/demo.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.859916 ANNarchy-4.7.2.3/examples/bar_learning/
--rw-r--r--   0 vitay      (501) staff       (20)     1844 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/bar_learning/BarLearning.py
--rw-r--r--   0 vitay      (501) staff       (20)     2104 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/examples/bar_learning/BarLearningGPU.py
--rw-r--r--   0 vitay      (501) staff       (20)     1610 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/examples/bar_learning/Viz.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.860384 ANNarchy-4.7.2.3/examples/bold_monitor/
--rw-r--r--   0 vitay      (501) staff       (20)     2529 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.3/examples/bold_monitor/BOLD.py
--rw-r--r--   0 vitay      (501) staff       (20)     3003 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.3/examples/bold_monitor/BOLD_two_inputs.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.860583 ANNarchy-4.7.2.3/examples/gap_junctions/
--rw-r--r--   0 vitay      (501) staff       (20)      888 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/gap_junctions/GapJunctions.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.860816 ANNarchy-4.7.2.3/examples/hodgkin_huxley/
--rw-r--r--   0 vitay      (501) staff       (20)     2496 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.3/examples/hodgkin_huxley/HodgkinHuxley.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.861264 ANNarchy-4.7.2.3/examples/homeostatic_stdp/
--rw-r--r--   0 vitay      (501) staff       (20)     5062 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/homeostatic_stdp/Ramp.py
--rw-r--r--   0 vitay      (501) staff       (20)     7059 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/homeostatic_stdp/SORF.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.861512 ANNarchy-4.7.2.3/examples/hybrid/
--rw-r--r--   0 vitay      (501) staff       (20)     2865 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/hybrid/Hybrid.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.862109 ANNarchy-4.7.2.3/examples/image/
--rw-r--r--   0 vitay      (501) staff       (20)     6193 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.3/examples/image/Image.py
--rw-r--r--   0 vitay      (501) staff       (20)     7210 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/examples/image/Webcam.ipynb
--rw-r--r--   0 vitay      (501) staff       (20)     2959 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/examples/image/Webcam.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.862337 ANNarchy-4.7.2.3/examples/izhikevich/
--rw-r--r--   0 vitay      (501) staff       (20)     1901 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/examples/izhikevich/Izhikevich.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.862522 ANNarchy-4.7.2.3/examples/multinetwork/
--rw-r--r--   0 vitay      (501) staff       (20)     1973 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.3/examples/multinetwork/MultiNetwork.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.863233 ANNarchy-4.7.2.3/examples/neural_field/
--rw-r--r--   0 vitay      (501) staff       (20)     1849 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/examples/neural_field/BubbleWorld.pyx
--rw-r--r--   0 vitay      (501) staff       (20)     1490 2020-03-10 16:42:35.000000 ANNarchy-4.7.2.3/examples/neural_field/NeuralField.py
--rw-r--r--   0 vitay      (501) staff       (20)     2281 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.3/examples/neural_field/Viz.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864318 ANNarchy-4.7.2.3/examples/pyNN/
--rw-r--r--   0 vitay      (501) staff       (20)     1644 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/AEIF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     2251 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/EIF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1427 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/IF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1361 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/IF_curr_alpha.py
--rw-r--r--   0 vitay      (501) staff       (20)     1316 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/non_linear_synapse.py
--rw-r--r--   0 vitay      (501) staff       (20)     2646 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/pyNN/short_term_plasticity2.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864461 ANNarchy-4.7.2.3/examples/refractoriness/
--rw-r--r--   0 vitay      (501) staff       (20)     1070 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/refractoriness/Refractoriness.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864602 ANNarchy-4.7.2.3/examples/simple_stdp/
--rw-r--r--   0 vitay      (501) staff       (20)     2208 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/simple_stdp/SimpleSTDPModel.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.864742 ANNarchy-4.7.2.3/examples/structural_plasticity/
--rw-r--r--   0 vitay      (501) staff       (20)     1923 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/structural_plasticity/StructuralPlasticity.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.866572 ANNarchy-4.7.2.3/examples/tensorboard/
--rw-r--r--   0 vitay      (501) staff       (20)  1014400 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.3/examples/tensorboard/BasalGanglia.ipynb
--rw-r--r--   0 vitay      (501) staff       (20)   208036 2021-07-27 06:26:43.000000 ANNarchy-4.7.2.3/examples/tensorboard/BayesianOptimization.ipynb
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.867072 ANNarchy-4.7.2.3/examples/tsodyks_markram/
--rw-r--r--   0 vitay      (501) staff       (20)     3872 2023-04-12 10:39:20.000000 ANNarchy-4.7.2.3/examples/tsodyks_markram/TsodyksMarkram.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.867883 ANNarchy-4.7.2.3/examples/vogels_abbott/
--rw-r--r--   0 vitay      (501) staff       (20)     1940 2020-09-29 13:24:31.000000 ANNarchy-4.7.2.3/examples/vogels_abbott/COBA.py
--rw-r--r--   0 vitay      (501) staff       (20)     1809 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.3/examples/vogels_abbott/CUBA.py
--rw-r--r--   0 vitay      (501) staff       (20)       82 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.3/requirements.txt
--rw-r--r--   0 vitay      (501) staff       (20)      101 2023-05-25 07:32:25.869173 ANNarchy-4.7.2.3/setup.cfg
--rw-r--r--   0 vitay      (501) staff       (20)    10946 2023-05-25 07:28:05.000000 ANNarchy-4.7.2.3/setup.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-05-25 07:32:25.868586 ANNarchy-4.7.2.3/tests/
--rw-r--r--   0 vitay      (501) staff       (20)     1122 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/tests/test_CUDA.py
--rw-r--r--   0 vitay      (501) staff       (20)     1062 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/tests/test_openmp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.3/tests/test_single_thread.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.043998 ANNarchy-4.7.2.4/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:36.993893 ANNarchy-4.7.2.4/ANNarchy/
+-rw-r--r--   0 vitay      (501) staff       (20)     1989 2023-06-23 04:23:35.000000 ANNarchy-4.7.2.4/ANNarchy/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.000110 ANNarchy-4.7.2.4/ANNarchy/core/
+-rw-r--r--   0 vitay      (501) staff       (20)    28001 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.4/ANNarchy/core/ConnectorMethods.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13851 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/core/Dendrite.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28338 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/core/Global.py
+-rw-r--r--   0 vitay      (501) staff       (20)    20797 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.4/ANNarchy/core/IO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    35087 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/core/Monitor.py
+-rw-r--r--   0 vitay      (501) staff       (20)    34541 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.4/ANNarchy/core/Network.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7309 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/core/NetworkManager.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8453 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/core/Neuron.py
+-rw-r--r--   0 vitay      (501) staff       (20)    32673 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.4/ANNarchy/core/Population.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12829 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/core/PopulationView.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6876 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/core/Profiler.py
+-rw-r--r--   0 vitay      (501) staff       (20)    65261 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.4/ANNarchy/core/Projection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8383 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.4/ANNarchy/core/Random.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10098 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/core/Simulate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    95368 2023-06-23 04:21:47.000000 ANNarchy-4.7.2.4/ANNarchy/core/SpecificPopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/core/SpecificProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5803 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/ANNarchy/core/Synapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3463 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/core/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/ANNarchy/core/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.000892 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/
+-rw-r--r--   0 vitay      (501) staff       (20)     1683 2022-05-18 09:30:59.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Connector.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)    21582 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Connector.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)      924 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Coordinates.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)     4941 2022-01-07 10:51:43.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Coordinates.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)     2866 2022-02-02 12:38:23.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Transformations.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/__init__.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)      405 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.001129 ANNarchy-4.7.2.4/ANNarchy/extensions/
+-rw-r--r--   0 vitay      (501) staff       (20)       21 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.001732 ANNarchy-4.7.2.4/ANNarchy/extensions/ann_to_snn_conversion/
+-rw-r--r--   0 vitay      (501) staff       (20)     9131 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3621 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
+-rw-r--r--   0 vitay      (501) staff       (20)       48 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.003103 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/
+-rw-r--r--   0 vitay      (501) staff       (20)    12839 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/AccProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2928 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/BoldModel.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10439 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/BoldMonitor.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15160 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/NormProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)    27888 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/PredefinedModels.py
+-rw-r--r--   0 vitay      (501) staff       (20)      386 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/bold/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.004644 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/
+-rw-r--r--   0 vitay      (501) staff       (20)    42897 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Convolve.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3005 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/ConvolveTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     9368 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Copy.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4502 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/CopyTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    24982 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Pooling.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14070 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/PoolingTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14093 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Transpose.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1583 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)      858 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.004975 ANNarchy-4.7.2.4/ANNarchy/extensions/diagonal/
+-rw-r--r--   0 vitay      (501) staff       (20)    16351 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/diagonal/DiagonalProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)       50 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/diagonal/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.005405 ANNarchy-4.7.2.4/ANNarchy/extensions/hybrid/
+-rw-r--r--   0 vitay      (501) staff       (20)    20781 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/hybrid/HybridPopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       72 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/hybrid/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.005803 ANNarchy-4.7.2.4/ANNarchy/extensions/image/
+-rw-r--r--   0 vitay      (501) staff       (20)     9944 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/image/ImagePopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       62 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/image/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.006222 ANNarchy-4.7.2.4/ANNarchy/extensions/tensorboard/
+-rw-r--r--   0 vitay      (501) staff       (20)    12742 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/tensorboard/Logger.py
+-rw-r--r--   0 vitay      (501) staff       (20)       26 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/tensorboard/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.006931 ANNarchy-4.7.2.4/ANNarchy/extensions/weightsharing/
+-rw-r--r--   0 vitay      (501) staff       (20)    51829 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/weightsharing/SharedProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)      206 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.4/ANNarchy/extensions/weightsharing/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.009001 ANNarchy-4.7.2.4/ANNarchy/generator/
+-rw-r--r--   0 vitay      (501) staff       (20)    42289 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/CodeGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    38169 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Compiler.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10654 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/MonitorGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.010634 ANNarchy-4.7.2.4/ANNarchy/generator/Population/
+-rw-r--r--   0 vitay      (501) staff       (20)    59484 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/CUDAGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    26498 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/CUDATemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    41946 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/OpenMPGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14427 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/OpenMPTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    20938 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/PopulationGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/SingleThreadGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13356 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/SingleThreadTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)      142 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Population/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.011652 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/
+-rw-r--r--   0 vitay      (501) staff       (20)    14883 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/CPP11Profile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8646 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/CUDAProfile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6963 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/PAPIProfile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3947 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/ProfileGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    31714 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/ProfileTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)      159 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Profile/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.013632 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.016451 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/
+-rw-r--r--   0 vitay      (501) staff       (20)    14633 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11089 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11052 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    36964 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13010 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12651 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19628 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11220 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15997 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15664 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8341 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/HYB.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10511 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1514 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    72468 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDAGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.018766 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/
+-rw-r--r--   0 vitay      (501) staff       (20)     8715 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13744 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37572 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8436 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8172 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6031 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19185 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4756 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5111 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    51527 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/LIL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/LIL_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4136 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1565 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    60579 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMPGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    49850 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/ProjectionGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.021367 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/
+-rw-r--r--   0 vitay      (501) staff       (20)     8717 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11194 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3413 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37503 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7292 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    17125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4489 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4792 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4570 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8588 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14808 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4607 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/HYB.py
+-rw-r--r--   0 vitay      (501) staff       (20)    45456 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/LIL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4120 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1671 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    57963 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThreadGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)      233 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Projection/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    54049 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/PyxGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15018 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Sanity.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.022819 ANNarchy-4.7.2.4/ANNarchy/generator/Template/
+-rw-r--r--   0 vitay      (501) staff       (20)    29830 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Template/BaseTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    16113 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Template/GlobalOperationTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2426 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Template/MakefileTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19390 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Template/MonitorTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14699 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Template/PyxTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Template/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15650 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/generator/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)       30 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.4/ANNarchy/generator/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.027853 ANNarchy-4.7.2.4/ANNarchy/include/
+-rw-r--r--   0 vitay      (501) staff       (20)    26125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/BSRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     6674 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/BSRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    17338 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.4/ANNarchy/include/COOMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8165 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/COOMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9119 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8274 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     7660 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrixCUDAT.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    22237 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrixT.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    21843 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/CSRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8971 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/CSRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    30517 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/DenseMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8778 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/DenseMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10925 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/DenseMatrixOffsets.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    32735 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/ELLMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9264 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/ELLMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    30967 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/ELLRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10305 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/ELLRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    19241 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/HYBMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     5284 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/HYBMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9991 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.4/ANNarchy/include/LILInvMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    37614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/LILMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    23769 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/PartitionedMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    25554 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/include/SELLMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9628 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/ANNarchy/include/SELLMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     1092 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.4/ANNarchy/include/Specific.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     1430 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.4/ANNarchy/include/helper_functions.hpp
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.029157 ANNarchy-4.7.2.4/ANNarchy/models/
+-rw-r--r--   0 vitay      (501) staff       (20)    45126 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.4/ANNarchy/models/Neurons.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11837 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.4/ANNarchy/models/Synapses.py
+-rw-r--r--   0 vitay      (501) staff       (20)      352 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/ANNarchy/models/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.032224 ANNarchy-4.7.2.4/ANNarchy/parser/
+-rw-r--r--   0 vitay      (501) staff       (20)    15017 2023-05-24 12:05:12.000000 ANNarchy-4.7.2.4/ANNarchy/parser/AnalyseNeuron.py
+-rw-r--r--   0 vitay      (501) staff       (20)    21586 2023-05-24 12:08:11.000000 ANNarchy-4.7.2.4/ANNarchy/parser/AnalyseSynapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14166 2023-05-24 12:05:32.000000 ANNarchy-4.7.2.4/ANNarchy/parser/CoupledEquations.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28868 2023-05-24 12:05:45.000000 ANNarchy-4.7.2.4/ANNarchy/parser/Equation.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28842 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/parser/Extraction.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4336 2022-12-05 16:13:02.000000 ANNarchy-4.7.2.4/ANNarchy/parser/Function.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6049 2022-12-05 16:13:18.000000 ANNarchy-4.7.2.4/ANNarchy/parser/ITE.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3032 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/ANNarchy/parser/ParserTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7633 2022-12-05 16:13:32.000000 ANNarchy-4.7.2.4/ANNarchy/parser/StringManipulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       86 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/ANNarchy/parser/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.033645 ANNarchy-4.7.2.4/ANNarchy/parser/report/
+-rw-r--r--   0 vitay      (501) staff       (20)    16861 2023-01-25 15:17:04.000000 ANNarchy-4.7.2.4/ANNarchy/parser/report/LatexParser.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22678 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/ANNarchy/parser/report/LatexReport.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15846 2021-04-01 06:34:12.000000 ANNarchy-4.7.2.4/ANNarchy/parser/report/MarkdownReport.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1985 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.4/ANNarchy/parser/report/Report.py
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/ANNarchy/parser/report/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.033735 ANNarchy-4.7.2.4/ANNarchy/thirdparty/
+-rw-r--r--   0 vitay      (501) staff       (20)    26759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/ANNarchy/thirdparty/randutils.hpp
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:36.994718 ANNarchy-4.7.2.4/ANNarchy.egg-info/
+-rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-06-23 04:26:36.000000 ANNarchy-4.7.2.4/ANNarchy.egg-info/PKG-INFO
+-rw-r--r--   0 vitay      (501) staff       (20)     8626 2023-06-23 04:26:36.000000 ANNarchy-4.7.2.4/ANNarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2023-06-23 04:26:36.000000 ANNarchy-4.7.2.4/ANNarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2021-04-13 07:32:27.000000 ANNarchy-4.7.2.4/ANNarchy.egg-info/not-zip-safe
+-rw-r--r--   0 vitay      (501) staff       (20)       36 2023-06-23 04:26:36.000000 ANNarchy-4.7.2.4/ANNarchy.egg-info/requires.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        9 2023-06-23 04:26:36.000000 ANNarchy-4.7.2.4/ANNarchy.egg-info/top_level.txt
+-rw-r--r--   0 vitay      (501) staff       (20)    18092 2017-07-25 21:20:59.000000 ANNarchy-4.7.2.4/LICENSE
+-rw-r--r--   0 vitay      (501) staff       (20)      274 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.4/MANIFEST.in
+-rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-06-23 04:26:37.044094 ANNarchy-4.7.2.4/PKG-INFO
+-rw-r--r--   0 vitay      (501) staff       (20)     1803 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/README.md
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:36.992512 ANNarchy-4.7.2.4/examples/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.034112 ANNarchy-4.7.2.4/examples/ann_to_snn/
+-rw-r--r--   0 vitay      (501) staff       (20)      991 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/examples/ann_to_snn/demo.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.034708 ANNarchy-4.7.2.4/examples/bar_learning/
+-rw-r--r--   0 vitay      (501) staff       (20)     1844 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/examples/bar_learning/BarLearning.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2104 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/examples/bar_learning/BarLearningGPU.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1610 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.4/examples/bar_learning/Viz.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.035147 ANNarchy-4.7.2.4/examples/bold_monitor/
+-rw-r--r--   0 vitay      (501) staff       (20)     2529 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.4/examples/bold_monitor/BOLD.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3003 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.4/examples/bold_monitor/BOLD_two_inputs.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.035318 ANNarchy-4.7.2.4/examples/gap_junctions/
+-rw-r--r--   0 vitay      (501) staff       (20)      888 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/examples/gap_junctions/GapJunctions.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.035512 ANNarchy-4.7.2.4/examples/hodgkin_huxley/
+-rw-r--r--   0 vitay      (501) staff       (20)     2496 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.4/examples/hodgkin_huxley/HodgkinHuxley.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.035993 ANNarchy-4.7.2.4/examples/homeostatic_stdp/
+-rw-r--r--   0 vitay      (501) staff       (20)     5062 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/homeostatic_stdp/Ramp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7059 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/homeostatic_stdp/SORF.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.036237 ANNarchy-4.7.2.4/examples/hybrid/
+-rw-r--r--   0 vitay      (501) staff       (20)     2865 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/hybrid/Hybrid.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.036822 ANNarchy-4.7.2.4/examples/image/
+-rw-r--r--   0 vitay      (501) staff       (20)     6193 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.4/examples/image/Image.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7210 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/examples/image/Webcam.ipynb
+-rw-r--r--   0 vitay      (501) staff       (20)     2959 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/examples/image/Webcam.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.037040 ANNarchy-4.7.2.4/examples/izhikevich/
+-rw-r--r--   0 vitay      (501) staff       (20)     1901 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.4/examples/izhikevich/Izhikevich.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.037257 ANNarchy-4.7.2.4/examples/multinetwork/
+-rw-r--r--   0 vitay      (501) staff       (20)     1973 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.4/examples/multinetwork/MultiNetwork.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.037955 ANNarchy-4.7.2.4/examples/neural_field/
+-rw-r--r--   0 vitay      (501) staff       (20)     1849 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/examples/neural_field/BubbleWorld.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)     1490 2020-03-10 16:42:35.000000 ANNarchy-4.7.2.4/examples/neural_field/NeuralField.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2281 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.4/examples/neural_field/Viz.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.039101 ANNarchy-4.7.2.4/examples/pyNN/
+-rw-r--r--   0 vitay      (501) staff       (20)     1644 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/pyNN/AEIF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2251 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/pyNN/EIF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1427 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/pyNN/IF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1361 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/pyNN/IF_curr_alpha.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1316 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/pyNN/non_linear_synapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2646 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/pyNN/short_term_plasticity2.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.039254 ANNarchy-4.7.2.4/examples/refractoriness/
+-rw-r--r--   0 vitay      (501) staff       (20)     1070 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/refractoriness/Refractoriness.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.039401 ANNarchy-4.7.2.4/examples/simple_stdp/
+-rw-r--r--   0 vitay      (501) staff       (20)     2208 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/examples/simple_stdp/SimpleSTDPModel.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.039550 ANNarchy-4.7.2.4/examples/structural_plasticity/
+-rw-r--r--   0 vitay      (501) staff       (20)     1923 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/examples/structural_plasticity/StructuralPlasticity.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.041331 ANNarchy-4.7.2.4/examples/tensorboard/
+-rw-r--r--   0 vitay      (501) staff       (20)  1014400 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.4/examples/tensorboard/BasalGanglia.ipynb
+-rw-r--r--   0 vitay      (501) staff       (20)   208036 2021-07-27 06:26:43.000000 ANNarchy-4.7.2.4/examples/tensorboard/BayesianOptimization.ipynb
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.042443 ANNarchy-4.7.2.4/examples/tsodyks_markram/
+-rw-r--r--   0 vitay      (501) staff       (20)     3872 2023-04-12 10:39:20.000000 ANNarchy-4.7.2.4/examples/tsodyks_markram/TsodyksMarkram.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.043012 ANNarchy-4.7.2.4/examples/vogels_abbott/
+-rw-r--r--   0 vitay      (501) staff       (20)     1940 2020-09-29 13:24:31.000000 ANNarchy-4.7.2.4/examples/vogels_abbott/COBA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1809 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.4/examples/vogels_abbott/CUBA.py
+-rw-r--r--   0 vitay      (501) staff       (20)       82 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.4/requirements.txt
+-rw-r--r--   0 vitay      (501) staff       (20)      101 2023-06-23 04:26:37.044381 ANNarchy-4.7.2.4/setup.cfg
+-rw-r--r--   0 vitay      (501) staff       (20)    10946 2023-06-23 04:23:49.000000 ANNarchy-4.7.2.4/setup.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-06-23 04:26:37.043819 ANNarchy-4.7.2.4/tests/
+-rw-r--r--   0 vitay      (501) staff       (20)     1122 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/tests/test_CUDA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1062 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/tests/test_openmp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.4/tests/test_single_thread.py
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/__init__.py` & `ANNarchy-4.7.2.4/ANNarchy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,11 +42,11 @@
 # if the script terminates
 import atexit
 atexit.register(check_profile_results)
 atexit.register(clear)
 
 # Version
 __version__ = '4.7'
-__release__ = '4.7.2.3'
+__release__ = '4.7.2.4'
 
 print( 'ANNarchy ' + __version__ + ' (' + __release__ + \
                     ') on ' + sys.platform + ' (' + os.name + ').' )
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/ConnectorMethods.py` & `ANNarchy-4.7.2.4/ANNarchy/core/ConnectorMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         idx_pre = weights.getcol(idx_post).indices
         w = weights.getcol(idx_post).data
         pr = [pre_ranks[i] for i in idx_pre]
         lil.add(post_ranks[idx_post], pr, w, [float(delays)])
 
     return lil
 
-def connect_from_file(self, filename, storage_format=None, storage_order=None):
+def connect_from_file(self, filename, pickle_encoding=None, storage_format=None, storage_order=None):
     """
     Builds the connectivity matrix using data saved using the Projection.save_connectivity() method (not save()!).
 
     Admissible file formats are compressed Numpy files (.npz), gunzipped binary text files (.gz) or binary text files.
 
     :param filename: file where the connections were saved.
 
@@ -504,15 +504,15 @@
     """
     # Create an empty LIL object
     lil = LILConnectivity()
 
     # Load the data
     from ANNarchy.core.IO import _load_connectivity_data
     try:
-        data = _load_connectivity_data(filename)
+        data = _load_connectivity_data(filename, pickle_encoding)
     except Exception as e:
         Global._print(e)
         Global._error('connect_from_file(): Unable to load the data', filename, 'into the projection.')
 
     # Load the LIL object
     try:
         # Size
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Dendrite.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Dendrite.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Global.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Global.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/IO.py` & `ANNarchy-4.7.2.4/ANNarchy/core/IO.py`

 * *Files 7% similar despite different names*

```diff
@@ -380,19 +380,20 @@
     :param populations: if True, population data will be saved (by default True)
     :param projections: if True, projection data will be saved (by default True)
 
     """
     data = _net_description(populations, projections, net_id)
     _save_data(filename, data)
 
-def _load_data(filename):
+def _load_data(filename, pickle_encoding):
     """
     Internally loads data contained in a given file.
 
     :param filename: path to the file.
+    :param pickle_encoding: if set to None the default is used, e.g. Python2 files ("latin1") or Python3 files ("ASCII")
     :return: A dictionary with the connectivity and synaptic variables if the file ``filename`` is available otherwise None is returned.
     """
     (_, fname) = os.path.split(filename)
     extension = os.path.splitext(fname)[1]
 
     if extension == '.mat':
         Global._error('Unable to load Matlab format.')
@@ -402,24 +403,30 @@
         try:
             import gzip
         except:
             Global._error('gzip is not installed.')
             return None
         try:
             with gzip.open(filename, mode = 'rb') as r_file:
-                desc = pickle.load(r_file)
+                if pickle_encoding is None:
+                    desc = pickle.load(r_file)
+                else:
+                    desc = pickle.load(r_file, encoding=pickle_encoding)
             return desc
         except Exception as e:
             Global._print('Unable to read the file ' + filename)
             Global._print(e)
             return None
 
     elif extension == '.npz':
         try:
-            data = np.load(filename, allow_pickle=True)
+            if pickle_encoding is None:
+                data = np.load(filename, allow_pickle=True)
+            else:
+                data = np.load(filename, allow_pickle=True, encoding=pickle_encoding)
             desc = {}
             for attribute in data.files:
                 # We need to distinguish two cases: 1) full network save
                 # or 2) single pop/proj. The first case leads to a dictionary
                 # of several objects. The latter to a dictionary containing all
                 # values.
                 if data[attribute].dtype == np.dtype('O'):
@@ -434,22 +441,25 @@
             Global._print('Unable to read the file ' + filename)
             Global._print(e)
             return None
 
     else:
         try:
             with open(filename, mode = 'rb') as r_file:
-                desc = pickle.load(r_file)
+                if pickle_encoding is None:
+                    desc = pickle.load(r_file)
+                else:
+                    desc = pickle.load(r_file, encoding=pickle_encoding)
             return desc
         except Exception as e:
             Global._print('Unable to read the file ' + filename)
             Global._print(e)
             return None
 
-def _load_connectivity_data(filename):
+def _load_connectivity_data(filename, pickle_encoding):
     """
     Internally loads data contained in a given file.
 
     :param filename: path to the file.
     :return: A dictionary with the connectivity and synaptic variables if the file ``filename`` is available otherwise None is returned.
     """
     (_, fname) = os.path.split(filename)
@@ -463,24 +473,30 @@
         try:
             import gzip
         except:
             Global._error('gzip is not installed.')
             return None
         try:
             with gzip.open(filename, mode = 'rb') as r_file:
-                desc = pickle.load(r_file)
+                if pickle_encoding is None:
+                    desc = pickle.load(r_file)
+                else:
+                    desc = pickle.load(r_file, encoding=pickle_encoding)
             return desc
         except Exception as e:
             Global._print('Unable to read the file ' + filename)
             Global._print(e)
             return None
 
     elif extension == '.npz':
         try:
-            data = np.load(filename, allow_pickle=True)
+            if pickle_encoding is None:
+                data = np.load(filename, allow_pickle=True)
+            else:
+                data = np.load(filename, allow_pickle=True, encoding=pickle_encoding)
             desc = {}
             for attribute in data.files:
                 # We need to distinguish two cases: 1) full network save
                 # or 2) single pop/proj. The first case leads to a dictionary
                 # of several objects. The latter to a dictionary containing all
                 # values.
                 desc[attribute] = data[attribute]
@@ -490,22 +506,25 @@
             Global._print('Unable to read the file ' + filename)
             Global._print(e)
             return None
 
     else:
         try:
             with open(filename, mode = 'rb') as r_file:
-                desc = pickle.load(r_file)
+                if pickle_encoding is None:
+                    desc = pickle.load(r_file)
+                else:
+                    desc = pickle.load(r_file, encoding=pickle_encoding)
             return desc
         except Exception as e:
             Global._print('Unable to read the file ' + filename)
             Global._print(e)
             return None
 
-def load(filename, populations=True, projections=True, net_id=0):
+def load(filename, populations=True, projections=True, pickle_encoding=None, net_id=0):
     """
     Loads a saved state of the network.
 
     **Warning:** Matlab data can not be loaded.
 
     Example:
 
@@ -513,17 +532,18 @@
     load('results/network.npz')
     ```
 
 
     :param filename: the filename with relative or absolute path.
     :param populations: if True, population data will be loaded (by default True)
     :param projections: if True, projection data will be loaded (by default True)
+    :param pickle_encoding: optional parameter provided to the pickle.load() method. If set to None the default is used.
     """
 
-    desc = _load_data(filename)
+    desc = _load_data(filename, pickle_encoding)
     if desc is None:
         return
 
     if 'time_step' in desc.keys():
         Global.set_current_step(desc['time_step'], net_id)
 
     if populations:
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Monitor.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Monitor.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Network.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Network.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,23 +553,24 @@
                     raise NotImplementedError
 
                 if target is not None:
                     raise NotImplementedError
 
             return res
 
-    def load(self, filename, populations=True, projections=True):
+    def load(self, filename, populations=True, projections=True, pickle_encoding=None):
         """
         Loads a saved state of the current network by calling ANNarchy.core.IO.load().
 
         :param filename: filename, may contain relative or absolute path.
         :param populations: if True, population data will be saved (by default True)
         :param projections: if True, projection data will be saved (by default True)
+        :param pickle_encoding: optional parameter provided to the pickle.load() method. If set to None the default is used.
         """
-        IO.load(filename=filename, populations=populations, projections=projections, net_id=self.id)
+        IO.load(filename=filename, populations=populations, projections=projections, pickle_encoding=pickle_encoding, net_id=self.id)
 
     def save(self, filename, populations=True, projections=True):
         """
         Saves the current network by calling ANNarchy.core.IO.save().
 
         :param filename: filename, may contain relative or absolute path.
         :param populations: if True, population data will be saved (by default True)
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/NetworkManager.py` & `ANNarchy-4.7.2.4/ANNarchy/core/NetworkManager.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Neuron.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Neuron.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Population.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Population.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
         ```
 
         """
         from ANNarchy.core.IO import _save_data
         _save_data(filename, self._data())
 
 
-    def load(self, filename):
+    def load(self, filename, pickle_encoding=None):
         """
         Load the saved state of the population by `Population.save()`.
 
         Warning: Matlab data can not be loaded.
 
         Example:
 
@@ -808,15 +808,15 @@
         pop.load('pop1.txt.gz')
         ```
 
         :param filename: the filename with relative or absolute path.
 
         """
         from ANNarchy.core.IO import _load_data
-        self._load_pop_data(_load_data(filename))
+        self._load_pop_data(_load_data(filename, pickle_encoding))
 
     def _load_pop_data(self, desc):
         """
         Updates the population with the stored data set.
         """
         if not 'attributes' in desc.keys():
             Global._error('Saved with a too old version of ANNarchy (< 4.2).', exit=True)
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/PopulationView.py` & `ANNarchy-4.7.2.4/ANNarchy/core/PopulationView.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Profiler.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Profiler.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Projection.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1309,15 +1309,15 @@
         proj.save('proj1.mat')
         ```
         """
         from ANNarchy.core.IO import _save_data
         _save_data(filename, self._data())
 
 
-    def load(self, filename):
+    def load(self, filename, pickle_encoding=None):
         """
         Loads the saved state of the projection by `Projection.save()`.
 
         Warning: Matlab data can not be loaded.
 
         Example:
 
@@ -1326,15 +1326,15 @@
         proj.load('proj1.txt')
         proj.load('proj1.txt.gz')
         ```
 
         :param filename: the file name with relative or absolute path.
         """
         from ANNarchy.core.IO import _load_connectivity_data
-        self._load_proj_data(_load_connectivity_data(filename))
+        self._load_proj_data(_load_connectivity_data(filename, pickle_encoding))
 
 
     def _load_proj_data(self, desc):
         """
         Updates the projection with the stored data set.
         """
         # Sanity check
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Random.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Random.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Simulate.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Simulate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/SpecificPopulation.py` & `ANNarchy-4.7.2.4/ANNarchy/core/SpecificPopulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1601,15 +1601,14 @@
             if self.initialized:
                 self.cyInstance.set_schedule( np.array(value) / Global.config['dt'] )
             else:
                 self.init['schedule'] = value
         elif name == 'rates':
             if self.initialized:
                 value = np.array(value)
-                print(value.shape)
                 if value.shape[0] != self.schedule.shape[0]:
                     Global._error("TimedPoissonPopulation: the first dimension of rates must match the schedule.")
                 if value.ndim > 2:
                     # we need to flatten the provided data
                     values = value.reshape( (value.shape[0], self.size) )
                     self.cyInstance.set_rates(values)
                 elif value.ndim == 2:
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/SpecificProjection.py` & `ANNarchy-4.7.2.4/ANNarchy/core/SpecificProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Synapse.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Synapse.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/Utils.py` & `ANNarchy-4.7.2.4/ANNarchy/core/Utils.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pxd` & `ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Connector.pxd`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Connector.pyx` & `ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Connector.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pxd` & `ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Coordinates.pxd`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Coordinates.pyx` & `ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Coordinates.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/core/cython_ext/Transformations.pyx` & `ANNarchy-4.7.2.4/ANNarchy/core/cython_ext/Transformations.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/AccProjection.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/bold/AccProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldModel.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/bold/BoldModel.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/BoldMonitor.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/bold/BoldMonitor.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/NormProjection.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/bold/NormProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/bold/PredefinedModels.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/bold/PredefinedModels.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Convolve.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Convolve.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/ConvolveTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/ConvolveTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Copy.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Copy.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/CopyTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/CopyTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Pooling.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Pooling.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/PoolingTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/PoolingTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Transpose.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Transpose.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/Utils.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/Utils.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/convolution/__init__.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/convolution/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/diagonal/DiagonalProjection.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/diagonal/DiagonalProjection.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/hybrid/HybridPopulation.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/hybrid/HybridPopulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/image/ImagePopulation.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/image/ImagePopulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/tensorboard/Logger.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/tensorboard/Logger.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/extensions/weightsharing/SharedProjection.py` & `ANNarchy-4.7.2.4/ANNarchy/extensions/weightsharing/SharedProjection.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,31 +76,28 @@
             Global._error('ANNarchy was not successfully installed.')
 
         lil = LILConnectivity()
         lil.max_delay = self.delays
         lil.uniform_delay = self.delays
         self.connector_name = "Shared weights"
         self.connector_description = "Shared weights"
-        self._store_connectivity(self._load_from_lil, (lil, ), self.delays)
+        self._store_connectivity(self._load_from_lil, (lil, ), self.delays, storage_format="lil", storage_order="post_to_pre")
 
     def _connect(self, module):
         """
         Builds up dendrites either from list or dictionary. Called by instantiate().
         """
         if not self._connection_method:
             Global._error('SharedProjection: The projection between ' + self.pre.name + ' and ' + self.post.name + ' is declared but not connected.')
 
 
         # Create the Cython instance
         proj = getattr(module, 'proj'+str(self.id)+'_wrapper')
         self.cyInstance = proj(self.weights, self.pre_coordinates)
 
-        # Define the list of postsynaptic neurons
-        self.post_ranks = list(range(self.post.size))
-
         # Set delays after instantiation
         if self.delays > 0.0:
             self.cyInstance.set_delay(self.delays/Global.config['dt'])
 
         return True
 
     def center(self, *args, **kwds):
@@ -919,31 +916,39 @@
             'access_connectivity_matrix': """
     // Accessor to connectivity data
     std::vector<int> get_post_rank() { return post_rank; }
     void set_post_rank(std::vector<int> ranks) { post_rank = ranks; }
     std::vector< std::vector<int> > get_pre_rank() { return pre_rank; }
     void set_pre_rank(std::vector< std::vector<int> > ranks) { pre_rank = ranks; }
     int dendrite_size(int n) { return pre_rank[n].size(); }
+    int nb_dendrites() { return post_rank.size(); }
 """ ,
 
             # Export the connectivity matrix
             'export_connectivity': """
         # Connectivity
         vector[int] get_post_rank()
         vector[vector[int]] get_pre_rank()
         void set_post_rank(vector[int])
         void set_pre_rank(vector[vector[int]])
+        int nb_dendrites()
 """,
 
+            'declare_parameters_variables': "",
+            'access_parameters_variables': "",
+
             # Arguments to the wrapper constructor
             'wrapper_args': "weights, coords",
 
             # Delays
             'wrapper_init_delay': "",
 
+            # Suppress calls like init_from_lil()
+            'wrapper_connector_call': "",
+
             # Initialize the wrapper connectivity matrix
             'wrapper_init_connectivity': """
         proj%(id_proj)s.set_post_rank(list(range(%(size_post)s)))
         proj%(id_proj)s.set_pre_rank(coords)
 """ % {'id_proj': self.id, 'size_post': self.post.size},
 
             # Wrapper access to connectivity matrix
@@ -957,15 +962,17 @@
 
             # Wrapper access to variables
             'wrapper_access_parameters_variables' : "",
 
             # Variables for the psp code
             'psp_prefix': """
         int rk_pre;
-        %(float_prec)s sum=0.0;""" % {'float_prec': Global.config['precision']}
+        %(float_prec)s sum=0.0;""" % {'float_prec': Global.config['precision']},
+
+            'clear_container': ""
         }
 
         # Kernel-based method: specify w with the correct dimension
         if kernel:
             self._specific_template['access_connectivity_matrix'] += """
     // Local parameter w
     %(type_w)s get_w() { return w; }
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/CodeGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/CodeGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Compiler.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Compiler.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/MonitorGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/MonitorGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDAGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/CUDAGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/CUDATemplates.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/CUDATemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/OpenMPGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/OpenMPTemplates.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/OpenMPTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/PopulationGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/PopulationGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/SingleThreadGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Population/SingleThreadTemplates.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Population/SingleThreadTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CPP11Profile.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Profile/CPP11Profile.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/CUDAProfile.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Profile/CUDAProfile.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/PAPIProfile.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Profile/PAPIProfile.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Profile/ProfileGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Profile/ProfileTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Profile/ProfileTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BSR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/BSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/COO.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/COO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/CSR_Vector.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/Dense.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/Dense_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/Dense_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/ELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/ELLR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/ELLR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/HYB.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/HYB.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/SELL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/SELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDA/__init__.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDA/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/CUDAGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/CUDAGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BSR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/BSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/COO.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/COO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR_P.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/Dense.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/Dense_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/ELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/ELLR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/ELLR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/LIL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/LIL_P.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/SELL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/SELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMP/__init__.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMP/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/OpenMPGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/OpenMPGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/ProjectionGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/ProjectionGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BSR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/BSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/COO.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/COO.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/CSR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/CSR_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense_PV.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/Dense_T.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/ELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/ELLR.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/ELLR.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/HYB.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/HYB.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/LIL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/LIL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/SELL.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/SELL.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThread/__init__.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThread/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Projection/SingleThreadGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Projection/SingleThreadGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/PyxGenerator.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/PyxGenerator.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Sanity.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Sanity.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Template/BaseTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Template/BaseTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Template/GlobalOperationTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Template/GlobalOperationTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Template/MakefileTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Template/MakefileTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Template/MonitorTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Template/MonitorTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Template/PyxTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Template/PyxTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/generator/Utils.py` & `ANNarchy-4.7.2.4/ANNarchy/generator/Utils.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/BSRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/BSRMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/BSRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/COOMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/COOMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/COOMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/COOMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixCUDAT.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrixCUDAT.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/CSRCMatrixT.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/CSRCMatrixT.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/CSRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/CSRMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/CSRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/DenseMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/DenseMatrixOffsets.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/DenseMatrixOffsets.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/ELLMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/ELLMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/ELLMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/ELLRMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/ELLRMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/ELLRMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/HYBMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/HYBMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/HYBMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/LILInvMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/LILInvMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/LILMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/LILMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/PartitionedMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/PartitionedMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrix.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/SELLMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/SELLMatrixCUDA.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/SELLMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/Specific.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/Specific.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/include/helper_functions.hpp` & `ANNarchy-4.7.2.4/ANNarchy/include/helper_functions.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/models/Neurons.py` & `ANNarchy-4.7.2.4/ANNarchy/models/Neurons.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/models/Synapses.py` & `ANNarchy-4.7.2.4/ANNarchy/models/Synapses.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseNeuron.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/AnalyseNeuron.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/AnalyseSynapse.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/AnalyseSynapse.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/CoupledEquations.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/CoupledEquations.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/Equation.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/Equation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/Extraction.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/Extraction.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/Function.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/Function.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/ITE.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/ITE.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/ParserTemplate.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/ParserTemplate.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/StringManipulation.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/StringManipulation.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexParser.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/report/LatexParser.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/report/LatexReport.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/report/LatexReport.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/report/MarkdownReport.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/report/MarkdownReport.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/parser/report/Report.py` & `ANNarchy-4.7.2.4/ANNarchy/parser/report/Report.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy/thirdparty/randutils.hpp` & `ANNarchy-4.7.2.4/ANNarchy/thirdparty/randutils.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/ANNarchy.egg-info/PKG-INFO` & `ANNarchy-4.7.2.4/ANNarchy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANNarchy
-Version: 4.7.2.3
+Version: 4.7.2.4
 Summary: Artificial Neural Networks architect
 Home-page: http://www.tu-chemnitz.de/informatik/KI/projects/ANNarchy/index.php
 Download-URL: https://bitbucket.org/annarchy/annarchy
 Author: Julien Vitay, Helge Uelo Dinkelbach and Fred Hamker
 Author-email: julien.vitay@informatik.tu-chemnitz.de
 License: GPLv2+
 Keywords: neural simulator
```

### Comparing `ANNarchy-4.7.2.3/ANNarchy.egg-info/SOURCES.txt` & `ANNarchy-4.7.2.4/ANNarchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/LICENSE` & `ANNarchy-4.7.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/PKG-INFO` & `ANNarchy-4.7.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANNarchy
-Version: 4.7.2.3
+Version: 4.7.2.4
 Summary: Artificial Neural Networks architect
 Home-page: http://www.tu-chemnitz.de/informatik/KI/projects/ANNarchy/index.php
 Download-URL: https://bitbucket.org/annarchy/annarchy
 Author: Julien Vitay, Helge Uelo Dinkelbach and Fred Hamker
 Author-email: julien.vitay@informatik.tu-chemnitz.de
 License: GPLv2+
 Keywords: neural simulator
```

### Comparing `ANNarchy-4.7.2.3/README.md` & `ANNarchy-4.7.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/ann_to_snn/demo.py` & `ANNarchy-4.7.2.4/examples/ann_to_snn/demo.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/bar_learning/BarLearning.py` & `ANNarchy-4.7.2.4/examples/bar_learning/BarLearning.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/bar_learning/BarLearningGPU.py` & `ANNarchy-4.7.2.4/examples/bar_learning/BarLearningGPU.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/bar_learning/Viz.py` & `ANNarchy-4.7.2.4/examples/bar_learning/Viz.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/bold_monitor/BOLD.py` & `ANNarchy-4.7.2.4/examples/bold_monitor/BOLD.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/bold_monitor/BOLD_two_inputs.py` & `ANNarchy-4.7.2.4/examples/bold_monitor/BOLD_two_inputs.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/gap_junctions/GapJunctions.py` & `ANNarchy-4.7.2.4/examples/gap_junctions/GapJunctions.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/hodgkin_huxley/HodgkinHuxley.py` & `ANNarchy-4.7.2.4/examples/hodgkin_huxley/HodgkinHuxley.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/homeostatic_stdp/Ramp.py` & `ANNarchy-4.7.2.4/examples/homeostatic_stdp/Ramp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/homeostatic_stdp/SORF.py` & `ANNarchy-4.7.2.4/examples/homeostatic_stdp/SORF.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/hybrid/Hybrid.py` & `ANNarchy-4.7.2.4/examples/hybrid/Hybrid.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/image/Image.py` & `ANNarchy-4.7.2.4/examples/image/Image.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/image/Webcam.ipynb` & `ANNarchy-4.7.2.4/examples/image/Webcam.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/image/Webcam.py` & `ANNarchy-4.7.2.4/examples/image/Webcam.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/izhikevich/Izhikevich.py` & `ANNarchy-4.7.2.4/examples/izhikevich/Izhikevich.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/multinetwork/MultiNetwork.py` & `ANNarchy-4.7.2.4/examples/multinetwork/MultiNetwork.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/neural_field/BubbleWorld.pyx` & `ANNarchy-4.7.2.4/examples/neural_field/BubbleWorld.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/neural_field/NeuralField.py` & `ANNarchy-4.7.2.4/examples/neural_field/NeuralField.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/neural_field/Viz.py` & `ANNarchy-4.7.2.4/examples/neural_field/Viz.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/pyNN/AEIF_cond_exp.py` & `ANNarchy-4.7.2.4/examples/pyNN/AEIF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/pyNN/EIF_cond_exp.py` & `ANNarchy-4.7.2.4/examples/pyNN/EIF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/pyNN/IF_cond_exp.py` & `ANNarchy-4.7.2.4/examples/pyNN/IF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/pyNN/IF_curr_alpha.py` & `ANNarchy-4.7.2.4/examples/pyNN/IF_curr_alpha.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/pyNN/non_linear_synapse.py` & `ANNarchy-4.7.2.4/examples/pyNN/non_linear_synapse.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/pyNN/short_term_plasticity2.py` & `ANNarchy-4.7.2.4/examples/pyNN/short_term_plasticity2.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/refractoriness/Refractoriness.py` & `ANNarchy-4.7.2.4/examples/refractoriness/Refractoriness.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/simple_stdp/SimpleSTDPModel.py` & `ANNarchy-4.7.2.4/examples/simple_stdp/SimpleSTDPModel.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/structural_plasticity/StructuralPlasticity.py` & `ANNarchy-4.7.2.4/examples/structural_plasticity/StructuralPlasticity.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/tensorboard/BasalGanglia.ipynb` & `ANNarchy-4.7.2.4/examples/tensorboard/BasalGanglia.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/tensorboard/BayesianOptimization.ipynb` & `ANNarchy-4.7.2.4/examples/tensorboard/BayesianOptimization.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/tsodyks_markram/TsodyksMarkram.py` & `ANNarchy-4.7.2.4/examples/tsodyks_markram/TsodyksMarkram.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/vogels_abbott/COBA.py` & `ANNarchy-4.7.2.4/examples/vogels_abbott/COBA.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/examples/vogels_abbott/CUBA.py` & `ANNarchy-4.7.2.4/examples/vogels_abbott/CUBA.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/setup.py` & `ANNarchy-4.7.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     'numpy',
     'scipy',
     'matplotlib',
     'cython',
     'sympy'
 ]
 
-release = '4.7.2.3'
+release = '4.7.2.4'
 print("Installing ANNarchy", release)
 py_version, py_major, python_include, python_libpath, cython_major = python_environment()
 print("\tPython", py_version, "(", sys.executable, ')')
 print("\tIncludes:", python_include)
 print("\tLibraries:", python_libpath)
 print("\tCython:", cython_major)
 print("\tNumpy:", np.get_include())
```

### Comparing `ANNarchy-4.7.2.3/tests/test_CUDA.py` & `ANNarchy-4.7.2.4/tests/test_CUDA.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/tests/test_openmp.py` & `ANNarchy-4.7.2.4/tests/test_openmp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.3/tests/test_single_thread.py` & `ANNarchy-4.7.2.4/tests/test_single_thread.py`

 * *Files identical despite different names*

