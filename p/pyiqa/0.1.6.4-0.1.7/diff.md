# Comparing `tmp/pyiqa-0.1.6.4.tar.gz` & `tmp/pyiqa-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiqa-0.1.6.4.tar", last modified: Mon Apr 17 18:50:01 2023, max compression
+gzip compressed data, was "dist/pyiqa-0.1.7.tar", last modified: Fri Jun 23 11:59:10 2023, max compression
```

## Comparing `pyiqa-0.1.6.4.tar` & `pyiqa-0.1.7.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    21165 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/LICENSE
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1717 2022-09-23 04:11:05.000000 pyiqa-0.1.6.4/LICENSE_NTU-S-Lab
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)       41 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/MANIFEST.in
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12233 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/PKG-INFO
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11357 2023-03-30 12:36:49.000000 pyiqa-0.1.6.4/README.md
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)        8 2023-04-17 18:44:53.000000 pyiqa-0.1.6.4/VERSION
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      322 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2137 2023-03-05 10:38:17.000000 pyiqa-0.1.6.4/pyiqa/api_helpers.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/archs/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      881 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8301 2023-04-01 06:45:12.000000 pyiqa-0.1.6.4/pyiqa/archs/ahiq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6053 2023-04-01 05:18:18.000000 pyiqa-0.1.6.4/pyiqa/archs/arch_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7158 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/brisque_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12397 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/ckdn_arch.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    25129 2023-01-11 18:50:33.000000 pyiqa-0.1.6.4/pyiqa/archs/clip_model.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     6636 2023-04-01 05:18:41.000000 pyiqa-0.1.6.4/pyiqa/archs/clipiqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2425 2022-11-21 12:29:26.000000 pyiqa-0.1.6.4/pyiqa/archs/cnniqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      387 2022-12-21 06:18:18.000000 pyiqa-0.1.6.4/pyiqa/archs/constants.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6126 2022-09-14 13:07:48.000000 pyiqa-0.1.6.4/pyiqa/archs/dbcnn_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5207 2023-03-05 10:40:20.000000 pyiqa-0.1.6.4/pyiqa/archs/dists_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10627 2023-04-01 05:16:09.000000 pyiqa-0.1.6.4/pyiqa/archs/fid_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18043 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/fsim_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6967 2023-03-29 10:09:20.000000 pyiqa-0.1.6.4/pyiqa/archs/func_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3471 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/gmsd_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7126 2023-04-01 05:19:52.000000 pyiqa-0.1.6.4/pyiqa/archs/hypernet_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12026 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/inception.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    23872 2023-04-01 05:20:23.000000 pyiqa-0.1.6.4/pyiqa/archs/iqt_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14538 2022-10-13 10:06:00.000000 pyiqa-0.1.6.4/pyiqa/archs/lpips_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11139 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/mad_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7328 2023-04-03 07:58:57.000000 pyiqa-0.1.6.4/pyiqa/archs/maniqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16352 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/maniqa_swin.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13552 2023-03-30 10:34:00.000000 pyiqa-0.1.6.4/pyiqa/archs/musiq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4013 2023-03-30 10:34:02.000000 pyiqa-0.1.6.4/pyiqa/archs/nima_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    19674 2023-04-01 05:20:50.000000 pyiqa-0.1.6.4/pyiqa/archs/niqe_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7050 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/nlpd_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16444 2023-03-29 13:57:08.000000 pyiqa-0.1.6.4/pyiqa/archs/nrqm_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2870 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/paq2piq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5467 2022-12-21 06:09:37.000000 pyiqa-0.1.6.4/pyiqa/archs/pieapp_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2663 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/psnr_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11245 2023-03-29 12:53:13.000000 pyiqa-0.1.6.4/pyiqa/archs/ssim_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14811 2023-02-22 14:19:42.000000 pyiqa-0.1.6.4/pyiqa/archs/tres_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    29869 2023-04-01 05:17:21.000000 pyiqa-0.1.6.4/pyiqa/archs/uranker_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18900 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/vif_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9905 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/vsi_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6508 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/wadiqam_arch.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/data/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4472 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4164 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/ava_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4390 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/bapps_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1812 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/data_sampler.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13252 2022-09-01 10:56:27.000000 pyiqa-0.1.6.4/pyiqa/data/data_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2678 2023-02-23 14:39:44.000000 pyiqa-0.1.6.4/pyiqa/data/flive_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3325 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/general_fr_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2726 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/general_nr_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2560 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/livechallenge_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7728 2022-09-01 10:54:53.000000 pyiqa-0.1.6.4/pyiqa/data/multiscale_trans_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4849 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/pieapp_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3201 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/pipal_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3131 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/prefetch_dataloader.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13759 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/transforms.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7620 2023-04-03 07:58:04.000000 pyiqa-0.1.6.4/pyiqa/default_model_configs.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/losses/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      716 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/losses/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4348 2022-09-01 10:48:31.000000 pyiqa-0.1.6.4/pyiqa/losses/iqa_losses.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2903 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/losses/loss_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7448 2022-09-01 10:47:19.000000 pyiqa-0.1.6.4/pyiqa/losses/losses.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      529 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10201 2023-03-29 12:41:27.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/functions.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2581 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/math_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12829 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/resize.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8063 2023-03-29 11:09:06.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/scfpyr_util.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/metrics/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      566 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/metrics/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2041 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/metrics/correlation_coefficient.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      270 2022-09-01 10:44:09.000000 pyiqa-0.1.6.4/pyiqa/metrics/other_metrics.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/models/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1007 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/models/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5767 2022-09-01 10:41:30.000000 pyiqa-0.1.6.4/pyiqa/models/bapps_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16067 2022-09-01 10:43:19.000000 pyiqa-0.1.6.4/pyiqa/models/base_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1737 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/models/dbcnn_model.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     8143 2023-01-11 18:50:33.000000 pyiqa-0.1.6.4/pyiqa/models/general_iqa_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1190 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/hypernet_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3089 2023-04-15 17:51:54.000000 pyiqa-0.1.6.4/pyiqa/models/inference_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3956 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/lr_scheduler.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2227 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/nima_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2302 2022-09-01 10:41:22.000000 pyiqa-0.1.6.4/pyiqa/models/pieapp_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9300 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/sr_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      975 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/wadiqam_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1720 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/test.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    11007 2023-01-11 18:50:33.000000 pyiqa-0.1.6.4/pyiqa/train.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2405 2022-09-01 11:01:29.000000 pyiqa-0.1.6.4/pyiqa/train_nsplits.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/utils/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      934 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7621 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/color_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2608 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/dist_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3345 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/download_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6017 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/file_client.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7261 2022-10-26 05:47:49.000000 pyiqa-0.1.6.4/pyiqa/utils/img_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7123 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/lmdb_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/logger.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4767 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/misc.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6474 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/options.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2185 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/registry.py
--rwxr-xr-x   0 cfchen   (25144) cfchen   (25144)      133 2023-04-17 18:49:59.000000 pyiqa-0.1.6.4/pyiqa/version.py
-drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa.egg-info/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12233 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/PKG-INFO
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2681 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/SOURCES.txt
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)        1 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/dependency_links.txt
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      170 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/requires.txt
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)        6 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/top_level.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      169 2023-03-29 17:32:51.000000 pyiqa-0.1.6.4/requirements.txt
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      333 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/setup.cfg
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3478 2023-03-29 17:15:09.000000 pyiqa-0.1.6.4/setup.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    21165 2022-08-14 08:39:50.000000 pyiqa-0.1.7/LICENSE
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1717 2022-09-23 04:11:05.000000 pyiqa-0.1.7/LICENSE_NTU-S-Lab
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)       41 2022-08-14 08:39:50.000000 pyiqa-0.1.7/MANIFEST.in
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    12231 2023-06-23 11:59:10.000000 pyiqa-0.1.7/PKG-INFO
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11357 2023-03-30 12:36:49.000000 pyiqa-0.1.7/README.md
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)        6 2023-06-23 11:42:59.000000 pyiqa-0.1.7/VERSION
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      322 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2137 2023-03-05 10:38:17.000000 pyiqa-0.1.7/pyiqa/api_helpers.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/archs/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      881 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8259 2023-04-21 11:24:04.000000 pyiqa-0.1.7/pyiqa/archs/ahiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6053 2023-04-01 05:18:18.000000 pyiqa-0.1.7/pyiqa/archs/arch_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7158 2023-05-25 19:19:58.000000 pyiqa-0.1.7/pyiqa/archs/brisque_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12397 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/ckdn_arch.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    25129 2023-01-11 18:50:33.000000 pyiqa-0.1.7/pyiqa/archs/clip_model.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     6636 2023-04-01 05:18:41.000000 pyiqa-0.1.7/pyiqa/archs/clipiqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1827 2023-06-09 14:01:56.000000 pyiqa-0.1.7/pyiqa/archs/clipscore_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2425 2022-11-21 12:29:26.000000 pyiqa-0.1.7/pyiqa/archs/cnniqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      387 2022-12-21 06:18:18.000000 pyiqa-0.1.7/pyiqa/archs/constants.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6126 2022-09-14 13:07:48.000000 pyiqa-0.1.7/pyiqa/archs/dbcnn_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5207 2023-03-05 10:40:20.000000 pyiqa-0.1.7/pyiqa/archs/dists_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1453 2023-06-16 07:14:54.000000 pyiqa-0.1.7/pyiqa/archs/entropy_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11009 2023-04-18 12:09:31.000000 pyiqa-0.1.7/pyiqa/archs/fid_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18043 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/fsim_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6967 2023-03-29 10:09:20.000000 pyiqa-0.1.7/pyiqa/archs/func_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3471 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/gmsd_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7126 2023-04-01 05:19:52.000000 pyiqa-0.1.7/pyiqa/archs/hypernet_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12026 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/inception.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    23872 2023-04-01 05:20:23.000000 pyiqa-0.1.7/pyiqa/archs/iqt_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14538 2022-10-13 10:06:00.000000 pyiqa-0.1.7/pyiqa/archs/lpips_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11139 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/mad_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7328 2023-04-03 07:58:57.000000 pyiqa-0.1.7/pyiqa/archs/maniqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16352 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/maniqa_swin.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13510 2023-05-25 16:57:19.000000 pyiqa-0.1.7/pyiqa/archs/musiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4013 2023-03-30 10:34:02.000000 pyiqa-0.1.7/pyiqa/archs/nima_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    19945 2023-06-01 04:20:40.000000 pyiqa-0.1.7/pyiqa/archs/niqe_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7050 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/nlpd_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16444 2023-03-29 13:57:08.000000 pyiqa-0.1.7/pyiqa/archs/nrqm_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2870 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/paq2piq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5467 2022-12-21 06:09:37.000000 pyiqa-0.1.7/pyiqa/archs/pieapp_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2663 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/psnr_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11184 2023-05-25 12:06:16.000000 pyiqa-0.1.7/pyiqa/archs/ssim_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14811 2023-02-22 14:19:42.000000 pyiqa-0.1.7/pyiqa/archs/tres_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    29869 2023-04-01 05:17:21.000000 pyiqa-0.1.7/pyiqa/archs/uranker_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18900 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/vif_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9938 2023-05-25 15:06:40.000000 pyiqa-0.1.7/pyiqa/archs/vsi_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6508 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/archs/wadiqam_arch.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/data/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4472 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4164 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/ava_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4390 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/bapps_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1812 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/data_sampler.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13252 2022-09-01 10:56:27.000000 pyiqa-0.1.7/pyiqa/data/data_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2678 2023-02-23 14:39:44.000000 pyiqa-0.1.7/pyiqa/data/flive_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3325 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/general_fr_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2726 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/general_nr_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2560 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/livechallenge_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7728 2022-09-01 10:54:53.000000 pyiqa-0.1.7/pyiqa/data/multiscale_trans_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4849 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/pieapp_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3201 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/pipal_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3131 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/prefetch_dataloader.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13759 2022-09-01 10:53:45.000000 pyiqa-0.1.7/pyiqa/data/transforms.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7891 2023-06-16 06:39:56.000000 pyiqa-0.1.7/pyiqa/default_model_configs.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/losses/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      716 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/losses/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4348 2022-09-01 10:48:31.000000 pyiqa-0.1.7/pyiqa/losses/iqa_losses.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2903 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/losses/loss_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7448 2022-09-01 10:47:19.000000 pyiqa-0.1.7/pyiqa/losses/losses.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/matlab_utils/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      529 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/matlab_utils/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10201 2023-03-29 12:41:27.000000 pyiqa-0.1.7/pyiqa/matlab_utils/functions.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2581 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/matlab_utils/math_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12829 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/matlab_utils/resize.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8057 2023-05-25 19:10:31.000000 pyiqa-0.1.7/pyiqa/matlab_utils/scfpyr_util.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/metrics/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      566 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/metrics/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2041 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/metrics/correlation_coefficient.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      270 2022-09-01 10:44:09.000000 pyiqa-0.1.7/pyiqa/metrics/other_metrics.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/models/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1007 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/models/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5767 2022-09-01 10:41:30.000000 pyiqa-0.1.7/pyiqa/models/bapps_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16067 2022-09-01 10:43:19.000000 pyiqa-0.1.7/pyiqa/models/base_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1737 2022-08-14 08:39:50.000000 pyiqa-0.1.7/pyiqa/models/dbcnn_model.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     8143 2023-01-11 18:50:33.000000 pyiqa-0.1.7/pyiqa/models/general_iqa_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1190 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/hypernet_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3166 2023-05-25 17:07:55.000000 pyiqa-0.1.7/pyiqa/models/inference_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3956 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/lr_scheduler.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2227 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/nima_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2302 2022-09-01 10:41:22.000000 pyiqa-0.1.7/pyiqa/models/pieapp_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9300 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/sr_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      975 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/models/wadiqam_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1720 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/test.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    11007 2023-01-11 18:50:33.000000 pyiqa-0.1.7/pyiqa/train.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2405 2022-09-01 11:01:29.000000 pyiqa-0.1.7/pyiqa/train_nsplits.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/utils/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      934 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7621 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/color_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2608 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/dist_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3345 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/download_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6017 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/file_client.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7261 2022-10-26 05:47:49.000000 pyiqa-0.1.7/pyiqa/utils/img_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7123 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/lmdb_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/logger.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4767 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/misc.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6474 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/options.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2185 2022-08-14 08:39:51.000000 pyiqa-0.1.7/pyiqa/utils/registry.py
+-rwxr-xr-x   0 cfchen   (25144) cfchen   (25144)      128 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa/version.py
+drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    12231 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/PKG-INFO
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     2739 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        1 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      170 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/requires.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        6 2023-06-23 11:59:10.000000 pyiqa-0.1.7/pyiqa.egg-info/top_level.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      169 2023-03-29 17:32:51.000000 pyiqa-0.1.7/requirements.txt
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      333 2023-06-23 11:59:10.000000 pyiqa-0.1.7/setup.cfg
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3478 2023-03-29 17:15:09.000000 pyiqa-0.1.7/setup.py
```

### Comparing `pyiqa-0.1.6.4/LICENSE` & `pyiqa-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/LICENSE_NTU-S-Lab` & `pyiqa-0.1.7/LICENSE_NTU-S-Lab`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/PKG-INFO` & `pyiqa-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiqa
-Version: 0.1.6.4
+Version: 0.1.7
 Summary: PyTorch Toolbox for Image Quality Assessment
 Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen
 Author-email: chaofenghust@gmail.com
 License: UNKNOWN
 Keywords: image quality assessment,pytorch
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyiqa Version: 0.1.6.4 Summary: PyTorch Toolbox for
+Metadata-Version: 2.1 Name: pyiqa Version: 0.1.7 Summary: PyTorch Toolbox for
 Image Quality Assessment Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen Author-email: chaofenghust@gmail.com License: UNKNOWN
 Keywords: image quality assessment,pytorch Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `pyiqa-0.1.6.4/README.md` & `pyiqa-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/api_helpers.py` & `pyiqa-0.1.7/pyiqa/api_helpers.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/__init__.py` & `pyiqa-0.1.7/pyiqa/archs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/ahiq_arch.py` & `pyiqa-0.1.7/pyiqa/archs/ahiq_arch.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,14 @@
         for p in model.parameters():
             p.requires_grad = False
 
     def preprocess(self, x):
         x = (x - self.default_mean.to(x)) / self.default_std.to(x)
         return x
 
-    @torch.no_grad()
     def get_vit_feature(self, x):
         self.vit(x)
         feat = torch.cat(
             (
                 self.save_output.outputs[x.device][0][:, 1:, :],
                 self.save_output.outputs[x.device][1][:, 1:, :],
                 self.save_output.outputs[x.device][2][:, 1:, :],
@@ -184,15 +183,14 @@
                 self.save_output.outputs[x.device][4][:, 1:, :],
             ),
             dim=2
         )
         self.save_output.clear(x.device)
         return feat
 
-    @torch.no_grad()
     def get_resnet_feature(self, x):
         self.resnet50(x)
         feat = torch.cat(
             (
                 self.save_output.outputs[x.device][0],
                 self.save_output.outputs[x.device][1],
                 self.save_output.outputs[x.device][2],
```

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/arch_util.py` & `pyiqa-0.1.7/pyiqa/archs/arch_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/brisque_arch.py` & `pyiqa-0.1.7/pyiqa/archs/brisque_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/ckdn_arch.py` & `pyiqa-0.1.7/pyiqa/archs/ckdn_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/clip_model.py` & `pyiqa-0.1.7/pyiqa/archs/clip_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/clipiqa_arch.py` & `pyiqa-0.1.7/pyiqa/archs/clipiqa_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/cnniqa_arch.py` & `pyiqa-0.1.7/pyiqa/archs/cnniqa_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/dbcnn_arch.py` & `pyiqa-0.1.7/pyiqa/archs/dbcnn_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/dists_arch.py` & `pyiqa-0.1.7/pyiqa/archs/dists_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/fid_arch.py` & `pyiqa-0.1.7/pyiqa/archs/fid_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,35 @@
 
 import torch
 from torch import nn
 import torchvision
 
 from .inception import InceptionV3
 from pyiqa.utils.download_util import load_file_from_url
-from pyiqa.utils.img_util import is_image_file
+from pyiqa.utils.img_util import is_image_file 
 from pyiqa.utils.registry import ARCH_REGISTRY
 
 default_model_urls = {
     'ffhq_clean_trainval70k_512.npz': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/ffhq_clean_trainval70k_512.npz',
     'ffhq_clean_trainval70k_512_kid.npz': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/ffhq_clean_trainval70k_512_kid.npz',
 }
 
 
+def get_file_paths(dir, max_dataset_size=float("inf"), followlinks=True):
+    images = []
+    assert os.path.isdir(dir), '%s is not a valid directory' % dir
+
+    for root, _, fnames in sorted(os.walk(dir, followlinks=followlinks)):
+        for fname in fnames:
+            if is_image_file(fname):
+                path = os.path.join(root, fname)
+                images.append(path)
+    return images[:min(max_dataset_size, len(images))]
+
+
 class ResizeDataset(torch.utils.data.Dataset):
     """
     A placeholder Dataset that enables parallelizing the resize operation
     using multiple CPU cores
     files: list of all files in the folder
     mode:
         - clean: use PIL resize before calculate features
@@ -180,15 +192,15 @@
                         mode="clean",
                         description="",
                         verbose=True,
                         ):
     r"""
     Compute the inception features for a folder of image files
     """
-    files = sorted([file for file in glob(os.path.join(fdir, '*')) if is_image_file(file)])
+    files = get_file_paths(fdir)
 
     if verbose:
         print(f"Found {len(files)} images in the folder {fdir}")
 
     dataset = ResizeDataset(files, mode=mode)
     dataloader = torch.utils.data.DataLoader(dataset,
                                              batch_size=batch_size, shuffle=False,
```

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/fsim_arch.py` & `pyiqa-0.1.7/pyiqa/archs/fsim_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/func_util.py` & `pyiqa-0.1.7/pyiqa/archs/func_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/gmsd_arch.py` & `pyiqa-0.1.7/pyiqa/archs/gmsd_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/hypernet_arch.py` & `pyiqa-0.1.7/pyiqa/archs/hypernet_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/inception.py` & `pyiqa-0.1.7/pyiqa/archs/inception.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/iqt_arch.py` & `pyiqa-0.1.7/pyiqa/archs/iqt_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/lpips_arch.py` & `pyiqa-0.1.7/pyiqa/archs/lpips_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/mad_arch.py` & `pyiqa-0.1.7/pyiqa/archs/mad_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/maniqa_arch.py` & `pyiqa-0.1.7/pyiqa/archs/maniqa_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/maniqa_swin.py` & `pyiqa-0.1.7/pyiqa/archs/maniqa_swin.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/musiq_arch.py` & `pyiqa-0.1.7/pyiqa/archs/musiq_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,18 +340,17 @@
         else:
             self.head = nn.Linear(hidden_size, num_class)
 
         if pretrained_model_path is not None:
             load_pretrained_network(self, pretrained_model_path, True)
 
     def forward(self, x, return_mos=True, return_dist=False):
-        if not self.training:
-            # normalize inputs to [-1, 1] as the official code
-            x = (x - 0.5) * 2
-            x = get_multiscale_patches(x, **self.data_preprocess_opts)
+        # normalize inputs to [-1, 1] as the official code
+        x = (x - 0.5) * 2
+        x = get_multiscale_patches(x, **self.data_preprocess_opts)
 
         assert len(x.shape) in [3, 4]
         if len(x.shape) == 4:
             b, num_crops, seq_len, dim = x.shape
             x = x.reshape(b * num_crops, seq_len, dim)
         else:
             b, seq_len, dim = x.shape
```

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/nima_arch.py` & `pyiqa-0.1.7/pyiqa/archs/nima_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/niqe_arch.py` & `pyiqa-0.1.7/pyiqa/archs/niqe_arch.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,16 +163,19 @@
     cov_pris_param = params['cov_prisparam']
     mu_pris_param = torch.from_numpy(mu_pris_param).to(img)
     cov_pris_param = torch.from_numpy(cov_pris_param).to(img)
 
     mu_pris_param = mu_pris_param.repeat(img.size(0), 1)
     cov_pris_param = cov_pris_param.repeat(img.size(0), 1, 1)
 
-    if test_y_channel and img.shape[1] == 3:
+    # NIQE only support gray image 
+    if img.shape[1] == 3:
         img = to_y_channel(img, 255, color_space)
+    elif img.shape[1] == 1:
+        img = img * 255
 
     img = diff_round(img)
     img = img.to(torch.float64)
 
     if crop_border != 0:
         img = img[..., crop_border:-crop_border, crop_border:-crop_border]
 
@@ -432,22 +435,22 @@
         self.color_space = color_space
         self.crop_border = crop_border
         if pretrained_model_path is not None:
             self.pretrained_model_path = pretrained_model_path
         else:
             self.pretrained_model_path = load_file_from_url(default_model_urls['url'])
 
-    def forward(self, X: torch.Tensor) -> torch.Tensor:
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         r"""Computation of NIQE metric.
-        Args:
-            X: An input tensor. Shape :math:`(N, C, H, W)`.
-        Returns:
-            Value of niqe metric in [0, 1] range.
+        Input:
+            x: An input tensor. Shape :math:`(N, C, H, W)`.
+        Output:
+            score (tensor): results of ilniqe metric, should be a positive real number. Shape :math:`(N, 1)`.
         """
-        score = calculate_niqe(X, self.crop_border, self.test_y_channel, self.pretrained_model_path, self.color_space)
+        score = calculate_niqe(x, self.crop_border, self.test_y_channel, self.pretrained_model_path, self.color_space)
         return score
 
 
 @ARCH_REGISTRY.register()
 class ILNIQE(torch.nn.Module):
     r"""Args:
         channels (int): Number of processed channel.
@@ -467,16 +470,17 @@
         self.channels = channels
         self.crop_border = crop_border
         if pretrained_model_path is not None:
             self.pretrained_model_path = pretrained_model_path
         else:
             self.pretrained_model_path = load_file_from_url(default_model_urls['ilniqe'])
 
-    def forward(self, X: torch.Tensor) -> torch.Tensor:
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         r"""Computation of NIQE metric.
-        Args:
-            X: An input tensor. Shape :math:`(N, C, H, W)`.
-        Returns:
-            Value of niqe metric in [0, 1] range.
+        Input:
+            x: An input tensor. Shape :math:`(N, C, H, W)`.
+        Output:
+            score (tensor): results of ilniqe metric, should be a positive real number. Shape :math:`(N, 1)`.
         """
-        score = calculate_ilniqe(X, self.crop_border, self.pretrained_model_path)
+        assert x.shape[1] == 3, 'ILNIQE only support input image with 3 channels'
+        score = calculate_ilniqe(x, self.crop_border, self.pretrained_model_path)
         return score
```

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/nlpd_arch.py` & `pyiqa-0.1.7/pyiqa/archs/nlpd_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/nrqm_arch.py` & `pyiqa-0.1.7/pyiqa/archs/nrqm_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/paq2piq_arch.py` & `pyiqa-0.1.7/pyiqa/archs/paq2piq_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/pieapp_arch.py` & `pyiqa-0.1.7/pyiqa/archs/pieapp_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/psnr_arch.py` & `pyiqa-0.1.7/pyiqa/archs/psnr_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/ssim_arch.py` & `pyiqa-0.1.7/pyiqa/archs/ssim_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         X = preprocess_rgb(X, self.test_y_channel, self.data_range, self.color_space)
         Y = preprocess_rgb(Y, self.test_y_channel, self.data_range, self.color_space) 
 
         score = ssim(X, Y, data_range=self.data_range, downsample=self.downsample)
         return score
 
 
-def ms_ssim(X, Y, win, data_range=1., downsample=False, test_y_channel=True, is_prod=True, color_space='yiq'):
+def ms_ssim(X, Y, win=None, data_range=1., downsample=False, test_y_channel=True, is_prod=True, color_space='yiq'):
     r"""Compute Multiscale structural similarity for a batch of images.
     Args:
         x: An input tensor. Shape :math:`(N, C, H, W)`.
         y: A target tensor. Shape :math:`(N, C, H, W)`.
         win: Window setting.
         downsample: Boolean, whether to downsample which mimics official SSIM matlab code.
         test_y_channel: Boolean, whether to use y channel on ycbcr.
@@ -132,16 +132,15 @@
         ssim_val, cs = ssim(
             X,
             Y,
             win=win,
             get_cs=True,
             downsample=downsample,
             data_range=data_range,
-            test_y_channel=test_y_channel,
-            color_space=color_space)
+            )
         mcs.append(cs)
         padding = (X.shape[2] % 2, X.shape[3] % 2)
         X = F.avg_pool2d(X, kernel_size=2, padding=padding)
         Y = F.avg_pool2d(Y, kernel_size=2, padding=padding)
 
     mcs = torch.stack(mcs, dim=0)
```

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/tres_arch.py` & `pyiqa-0.1.7/pyiqa/archs/tres_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/uranker_arch.py` & `pyiqa-0.1.7/pyiqa/archs/uranker_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/vif_arch.py` & `pyiqa-0.1.7/pyiqa/archs/vif_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/vsi_arch.py` & `pyiqa-0.1.7/pyiqa/archs/vsi_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         Image Quality Assessment," IEEE Transactions on Image Processing, vol. 23, no. 10,
         pp. 4270-4281, Oct. 2014, doi: 10.1109/TIP.2014.2346028
         https://ieeexplore.ieee.org/document/6873260
 
     Note:
         The original method supports only RGB image.
     """
-
+    x, y = x.double(), y.double()
     if x.size(1) == 1:
         x = x.repeat(1, 3, 1, 1)
         y = y.repeat(1, 3, 1, 1)
         warnings.warn('The original VSI supports only RGB images. The input images were converted to RGB by copying '
                       'the grey channel 3 times.')
 
     # Scale to [0, 255] range to match scale of constant
```

### Comparing `pyiqa-0.1.6.4/pyiqa/archs/wadiqam_arch.py` & `pyiqa-0.1.7/pyiqa/archs/wadiqam_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/__init__.py` & `pyiqa-0.1.7/pyiqa/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/ava_dataset.py` & `pyiqa-0.1.7/pyiqa/data/ava_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/bapps_dataset.py` & `pyiqa-0.1.7/pyiqa/data/bapps_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/data_sampler.py` & `pyiqa-0.1.7/pyiqa/data/data_sampler.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/data_util.py` & `pyiqa-0.1.7/pyiqa/data/data_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/flive_dataset.py` & `pyiqa-0.1.7/pyiqa/data/flive_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/general_fr_dataset.py` & `pyiqa-0.1.7/pyiqa/data/general_fr_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/general_nr_dataset.py` & `pyiqa-0.1.7/pyiqa/data/general_nr_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/livechallenge_dataset.py` & `pyiqa-0.1.7/pyiqa/data/livechallenge_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/multiscale_trans_util.py` & `pyiqa-0.1.7/pyiqa/data/multiscale_trans_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/pieapp_dataset.py` & `pyiqa-0.1.7/pyiqa/data/pieapp_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/pipal_dataset.py` & `pyiqa-0.1.7/pyiqa/data/pipal_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/prefetch_dataloader.py` & `pyiqa-0.1.7/pyiqa/data/prefetch_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/data/transforms.py` & `pyiqa-0.1.7/pyiqa/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/default_model_configs.py` & `pyiqa-0.1.7/pyiqa/default_model_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,9 +334,21 @@
         'metric_mode': 'NR',
     },
     'uranker': {
         'metric_opts': {
             'type': 'URanker',
         },
         'metric_mode': 'NR',
+    },
+    'clipscore': {
+        'metric_opts': {
+            'type': 'CLIPScore',
+        },
+        'metric_mode': 'NR', # Caption image similarity
+    },
+    'entropy': {
+        'metric_opts': {
+            'type': 'Entropy',
+        },
+        'metric_mode': 'NR',
     }
 })
```

### Comparing `pyiqa-0.1.6.4/pyiqa/losses/__init__.py` & `pyiqa-0.1.7/pyiqa/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/losses/iqa_losses.py` & `pyiqa-0.1.7/pyiqa/losses/iqa_losses.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/losses/loss_util.py` & `pyiqa-0.1.7/pyiqa/losses/loss_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/losses/losses.py` & `pyiqa-0.1.7/pyiqa/losses/losses.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/matlab_utils/__init__.py` & `pyiqa-0.1.7/pyiqa/matlab_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/matlab_utils/functions.py` & `pyiqa-0.1.7/pyiqa/matlab_utils/functions.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/matlab_utils/math_util.py` & `pyiqa-0.1.7/pyiqa/matlab_utils/math_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/matlab_utils/resize.py` & `pyiqa-0.1.7/pyiqa/matlab_utils/resize.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/matlab_utils/scfpyr_util.py` & `pyiqa-0.1.7/pyiqa/matlab_utils/scfpyr_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         self.scale_factor = scale_factor
         self.device = torch.device('cpu') if device is None else device
 
         # Cache constants
         self.lutsize = 1024
         self.Xcosn = np.pi * np.array(range(-(2 * self.lutsize + 1), (self.lutsize + 2))) / self.lutsize
         self.alpha = (self.Xcosn + np.pi) % (2 * np.pi) - np.pi
-        self.complex_fact_construct = np.power(np.complex(0, -1), self.nbands - 1)
-        self.complex_fact_reconstruct = np.power(np.complex(0, 1), self.nbands - 1)
+        self.complex_fact_construct = np.power(complex(0, -1), self.nbands - 1)
+        self.complex_fact_reconstruct = np.power(complex(0, 1), self.nbands - 1)
 
     ################################################################################
     # Construction of Steerable Pyramid
 
     def build(self, im_batch):
         ''' Decomposes a batch of images into a complex steerable pyramid.
         The pyramid typically has ~4 levels and 4-8 orientations.
```

### Comparing `pyiqa-0.1.6.4/pyiqa/metrics/__init__.py` & `pyiqa-0.1.7/pyiqa/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/metrics/correlation_coefficient.py` & `pyiqa-0.1.7/pyiqa/metrics/correlation_coefficient.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/__init__.py` & `pyiqa-0.1.7/pyiqa/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/bapps_model.py` & `pyiqa-0.1.7/pyiqa/models/bapps_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/base_model.py` & `pyiqa-0.1.7/pyiqa/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/dbcnn_model.py` & `pyiqa-0.1.7/pyiqa/models/dbcnn_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/general_iqa_model.py` & `pyiqa-0.1.7/pyiqa/models/general_iqa_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/hypernet_model.py` & `pyiqa-0.1.7/pyiqa/models/hypernet_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/inference_model.py` & `pyiqa-0.1.7/pyiqa/models/inference_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,10 +76,12 @@
 
                 if self.metric_mode == 'FR':
                     output = self.net(target.to(self.device), ref.to(self.device), **kwargs)
                 elif self.metric_mode == 'NR':
                     output = self.net(target.to(self.device), **kwargs)
 
         if self.as_loss:
+            if isinstance(output, tuple):
+                output = output[0]
             return weight_reduce_loss(output, self.loss_weight, self.loss_reduction)
         else:
             return output
```

### Comparing `pyiqa-0.1.6.4/pyiqa/models/lr_scheduler.py` & `pyiqa-0.1.7/pyiqa/models/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/nima_model.py` & `pyiqa-0.1.7/pyiqa/models/nima_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/pieapp_model.py` & `pyiqa-0.1.7/pyiqa/models/pieapp_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/sr_model.py` & `pyiqa-0.1.7/pyiqa/models/sr_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/models/wadiqam_model.py` & `pyiqa-0.1.7/pyiqa/models/wadiqam_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/test.py` & `pyiqa-0.1.7/pyiqa/test.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/train.py` & `pyiqa-0.1.7/pyiqa/train.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/train_nsplits.py` & `pyiqa-0.1.7/pyiqa/train_nsplits.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/__init__.py` & `pyiqa-0.1.7/pyiqa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/color_util.py` & `pyiqa-0.1.7/pyiqa/utils/color_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/dist_util.py` & `pyiqa-0.1.7/pyiqa/utils/dist_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/download_util.py` & `pyiqa-0.1.7/pyiqa/utils/download_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/file_client.py` & `pyiqa-0.1.7/pyiqa/utils/file_client.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/img_util.py` & `pyiqa-0.1.7/pyiqa/utils/img_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/lmdb_util.py` & `pyiqa-0.1.7/pyiqa/utils/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/logger.py` & `pyiqa-0.1.7/pyiqa/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/misc.py` & `pyiqa-0.1.7/pyiqa/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/options.py` & `pyiqa-0.1.7/pyiqa/utils/options.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa/utils/registry.py` & `pyiqa-0.1.7/pyiqa/utils/registry.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.4/pyiqa.egg-info/PKG-INFO` & `pyiqa-0.1.7/pyiqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiqa
-Version: 0.1.6.4
+Version: 0.1.7
 Summary: PyTorch Toolbox for Image Quality Assessment
 Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen
 Author-email: chaofenghust@gmail.com
 License: UNKNOWN
 Keywords: image quality assessment,pytorch
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyiqa Version: 0.1.6.4 Summary: PyTorch Toolbox for
+Metadata-Version: 2.1 Name: pyiqa Version: 0.1.7 Summary: PyTorch Toolbox for
 Image Quality Assessment Home-page: https://github.com/chaofengc/IQA-PyTorch
 Author: Chaofeng Chen Author-email: chaofenghust@gmail.com License: UNKNOWN
 Keywords: image quality assessment,pytorch Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `pyiqa-0.1.6.4/pyiqa.egg-info/SOURCES.txt` & `pyiqa-0.1.7/pyiqa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 pyiqa/archs/__init__.py
 pyiqa/archs/ahiq_arch.py
 pyiqa/archs/arch_util.py
 pyiqa/archs/brisque_arch.py
 pyiqa/archs/ckdn_arch.py
 pyiqa/archs/clip_model.py
 pyiqa/archs/clipiqa_arch.py
+pyiqa/archs/clipscore_arch.py
 pyiqa/archs/cnniqa_arch.py
 pyiqa/archs/constants.py
 pyiqa/archs/dbcnn_arch.py
 pyiqa/archs/dists_arch.py
+pyiqa/archs/entropy_arch.py
 pyiqa/archs/fid_arch.py
 pyiqa/archs/fsim_arch.py
 pyiqa/archs/func_util.py
 pyiqa/archs/gmsd_arch.py
 pyiqa/archs/hypernet_arch.py
 pyiqa/archs/inception.py
 pyiqa/archs/iqt_arch.py
```

### Comparing `pyiqa-0.1.6.4/setup.py` & `pyiqa-0.1.7/setup.py`

 * *Files identical despite different names*

