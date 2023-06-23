# Comparing `tmp/skyplane-nightly-0.2.1.dev20230312.tar.gz` & `tmp/skyplane_nightly-0.3.2.dev20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyplane-nightly-0.2.1.dev20230312.tar", max compression
+gzip compressed data, was "skyplane_nightly-0.3.2.dev20230622.tar", max compression
```

## Comparing `skyplane-nightly-0.2.1.dev20230312.tar` & `skyplane_nightly-0.3.2.dev20230622.tar`

### file list

```diff
@@ -1,86 +1,100 @@
--rw-r--r--   0        0        0    11357 2023-03-12 23:45:09.447308 skyplane-nightly-0.2.1.dev20230312/LICENSE
--rw-r--r--   0        0        0     6784 2023-03-12 23:45:09.447308 skyplane-nightly-0.2.1.dev20230312/README.md
--rw-r--r--   0        0        0     3083 2023-03-12 23:47:22.094913 skyplane-nightly-0.2.1.dev20230312/pyproject.toml
--rw-r--r--   0        0        0      590 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/__init__.py
--rw-r--r--   0        0        0     6762 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/client.py
--rw-r--r--   0        0        0     1849 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/config.py
--rw-r--r--   0        0        0    14603 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/dataplane.py
--rw-r--r--   0        0        0    13485 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/provisioner.py
--rw-r--r--   0        0        0    13832 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/tracker.py
--rw-r--r--   0        0        0    26659 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/transfer_job.py
--rw-r--r--   0        0        0    14318 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/api/usage.py
--rw-r--r--   0        0        0      811 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/cert.py
--rw-r--r--   0        0        0     2868 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/chunk_store.py
--rw-r--r--   0        0        0    13219 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_daemon.py
--rw-r--r--   0        0        0    13617 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_daemon_api.py
--rw-r--r--   0        0        0     3971 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_program.py
--rw-r--r--   0        0        0     3526 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_queue.py
--rw-r--r--   0        0        0    21966 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/operators/gateway_operator.py
--rw-r--r--   0        0        0     8277 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/operators/gateway_receiver.py
--rw-r--r--   0        0        0     5645 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/chunk.py
--rw-r--r--   0        0        0     3267 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli.py
--rw-r--r--   0        0        0    16801 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_cloud.py
--rw-r--r--   0        0        0     1678 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_config.py
--rw-r--r--   0        0        0    20363 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_init.py
--rw-r--r--   0        0        0    25696 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_transfer.py
--rw-r--r--   0        0        0      461 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/__init__.py
--rw-r--r--   0        0        0    21372 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/cli_profile.py
--rw-r--r--   0        0        0     1757 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/cli_query.py
--rw-r--r--   0        0        0     7459 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/provision.py
--rw-r--r--   0        0        0     3100 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/impl/common.py
--rw-r--r--   0        0        0     4678 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/impl/cp_replicate_fallback.py
--rw-r--r--   0        0        0     2767 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/cli/impl/progress_bar.py
--rw-r--r--   0        0        0      954 2023-03-12 23:45:09.467308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/__init__.py
--rw-r--r--   0        0        0     4224 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_auth.py
--rw-r--r--   0        0        0    11438 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_cloud_provider.py
--rw-r--r--   0        0        0     4315 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_key_manager.py
--rw-r--r--   0        0        0    11509 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_network.py
--rw-r--r--   0        0        0     1606 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_pricing.py
--rw-r--r--   0        0        0     6256 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_server.py
--rw-r--r--   0        0        0     6823 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/azure/azure_auth.py
--rw-r--r--   0        0        0    20635 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/azure/azure_cloud_provider.py
--rw-r--r--   0        0        0     7418 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/azure/azure_server.py
--rw-r--r--   0        0        0     3037 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/cloud_provider.py
--rw-r--r--   0        0        0     2883 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/const_cmds.py
--rw-r--r--   0        0        0    10830 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_auth.py
--rw-r--r--   0        0        0     9237 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_cloud_provider.py
--rw-r--r--   0        0        0     2462 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_key_manager.py
--rw-r--r--   0        0        0     5365 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_network.py
--rw-r--r--   0        0        0     2758 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_pricing.py
--rw-r--r--   0        0        0     5094 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_server.py
--rw-r--r--   0        0        0      937 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/key_utils.py
--rw-r--r--   0        0        0    16115 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/compute/server.py
--rw-r--r--   0        0        0     9062 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/config.py
--rw-r--r--   0        0        0      950 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/config_paths.py
--rw-r--r--   0        0        0        0 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/data/__init__.py
--rw-r--r--   0        0        0    15856 2023-03-12 23:45:09.471308 skyplane-nightly-0.2.1.dev20230312/skyplane/data/aws_transfer_costs.csv
--rwxr-xr-x   0        0        0  3684176 2023-03-12 23:45:09.483308 skyplane-nightly-0.2.1.dev20230312/skyplane/data/throughput.csv
--rw-r--r--   0        0        0     2879 2023-03-12 23:45:09.483308 skyplane-nightly-0.2.1.dev20230312/skyplane/exceptions.py
--rw-r--r--   0        0        0      811 2023-03-12 23:45:09.483308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/cert.py
--rw-r--r--   0        0        0     6322 2023-03-12 23:45:09.483308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/chunk_store.py
--rw-r--r--   0        0        0     9548 2023-03-12 23:45:09.483308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/gateway_daemon.py
--rw-r--r--   0        0        0    10523 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/gateway_daemon_api.py
--rw-r--r--   0        0        0     8352 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/gateway_obj_store.py
--rw-r--r--   0        0        0     8105 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/gateway_receiver.py
--rw-r--r--   0        0        0    10532 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway/gateway_sender.py
--rw-r--r--   0        0        0       37 2023-03-12 23:47:22.090913 skyplane-nightly-0.2.1.dev20230312/skyplane/gateway_version.py
--rw-r--r--   0        0        0     8273 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/azure_blob_interface.py
--rw-r--r--   0        0        0     2855 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/azure_storage_account_interface.py
--rw-r--r--   0        0        0    11831 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/gcs_interface.py
--rw-r--r--   0        0        0     4475 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/object_store_interface.py
--rw-r--r--   0        0        0    10226 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/s3_interface.py
--rw-r--r--   0        0        0     4521 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/planner/planner.py
--rw-r--r--   0        0        0    18125 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/planner/solver.py
--rw-r--r--   0        0        0     6501 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/planner/solver_ilp.py
--rw-r--r--   0        0        0     1996 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/planner/solver_ron.py
--rw-r--r--   0        0        0     8761 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/planner/topology.py
--rw-r--r--   0        0        0      846 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/cache.py
--rw-r--r--   0        0        0      617 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/definitions.py
--rw-r--r--   0        0        0     2486 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/fn.py
--rw-r--r--   0        0        0     1384 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/imports.py
--rw-r--r--   0        0        0     2131 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/logger.py
--rw-r--r--   0        0        0     2156 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/path.py
--rw-r--r--   0        0        0     1160 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/retry.py
--rw-r--r--   0        0        0      612 2023-03-12 23:45:09.487308 skyplane-nightly-0.2.1.dev20230312/skyplane/utils/timer.py
--rw-r--r--   0        0        0     9759 1970-01-01 00:00:00.000000 skyplane-nightly-0.2.1.dev20230312/setup.py
--rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 skyplane-nightly-0.2.1.dev20230312/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-22 16:57:49.396748 skyplane_nightly-0.3.2.dev20230622/LICENSE
+-rw-r--r--   0        0        0     7221 2023-06-22 16:57:49.396748 skyplane_nightly-0.3.2.dev20230622/README.md
+-rw-r--r--   0        0        0     3669 2023-06-22 16:58:56.456930 skyplane_nightly-0.3.2.dev20230622/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/__init__.py
+-rw-r--r--   0        0        0     4331 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/client.py
+-rw-r--r--   0        0        0     3040 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/config.py
+-rw-r--r--   0        0        0    14897 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/dataplane.py
+-rw-r--r--   0        0        0     2081 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/obj_store.py
+-rw-r--r--   0        0        0     6616 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/pipeline.py
+-rw-r--r--   0        0        0    15091 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/provisioner.py
+-rw-r--r--   0        0        0    17597 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/tracker.py
+-rw-r--r--   0        0        0    39032 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/transfer_job.py
+-rw-r--r--   0        0        0    14502 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/api/usage.py
+-rw-r--r--   0        0        0     5726 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/chunk.py
+-rw-r--r--   0        0        0     3317 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli.py
+-rw-r--r--   0        0        0    18045 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_cloud.py
+-rw-r--r--   0        0        0     1678 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_config.py
+-rw-r--r--   0        0        0    26670 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_init.py
+-rw-r--r--   0        0        0    24575 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_transfer.py
+-rw-r--r--   0        0        0      461 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/__init__.py
+-rw-r--r--   0        0        0    23462 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/cli_profile.py
+-rw-r--r--   0        0        0     1757 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/cli_query.py
+-rw-r--r--   0        0        0     9215 2023-06-22 16:57:49.412748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/provision.py
+-rw-r--r--   0        0        0     3100 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/impl/common.py
+-rw-r--r--   0        0        0     4678 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/impl/cp_replicate_fallback.py
+-rw-r--r--   0        0        0     3071 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/cli/impl/progress_bar.py
+-rw-r--r--   0        0        0     1247 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/__init__.py
+-rw-r--r--   0        0        0     5908 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_auth.py
+-rw-r--r--   0        0        0    11591 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_cloud_provider.py
+-rw-r--r--   0        0        0     4315 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_key_manager.py
+-rw-r--r--   0        0        0    11509 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_network.py
+-rw-r--r--   0        0        0     1606 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_pricing.py
+-rw-r--r--   0        0        0     6294 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_server.py
+-rw-r--r--   0        0        0     9526 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/azure/azure_auth.py
+-rw-r--r--   0        0        0    20681 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/azure/azure_cloud_provider.py
+-rw-r--r--   0        0        0     7503 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/azure/azure_server.py
+-rw-r--r--   0        0        0     3564 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/cloud_provider.py
+-rw-r--r--   0        0        0     2883 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/const_cmds.py
+-rw-r--r--   0        0        0    12043 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_auth.py
+-rw-r--r--   0        0        0     9355 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_cloud_provider.py
+-rw-r--r--   0        0        0     2462 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_key_manager.py
+-rw-r--r--   0        0        0     5365 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_network.py
+-rw-r--r--   0        0        0     2786 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_pricing.py
+-rw-r--r--   0        0        0     5151 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_server.py
+-rw-r--r--   0        0        0      211 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
+-rw-r--r--   0        0        0        0 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_gen2/__init__.py
+-rw-r--r--   0        0        0     2242 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_gen2/config.py
+-rw-r--r--   0        0        0      877 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_gen2/constants.py
+-rw-r--r--   0        0        0     5353 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_gen2/ssh_client.py
+-rw-r--r--   0        0        0      710 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_gen2/utils.py
+-rw-r--r--   0        0        0    40464 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibm_gen2/vpc_backend.py
+-rw-r--r--   0        0        0     5320 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibmcloud_auth.py
+-rw-r--r--   0        0        0     2851 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibmcloud_provider.py
+-rw-r--r--   0        0        0     3522 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/ibmcloud/ibmcloud_server.py
+-rw-r--r--   0        0        0      937 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/key_utils.py
+-rw-r--r--   0        0        0    17426 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/compute/server.py
+-rw-r--r--   0        0        0    13589 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/config.py
+-rw-r--r--   0        0        0     1229 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/config_paths.py
+-rw-r--r--   0        0        0        0 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/data/__init__.py
+-rw-r--r--   0        0        0    19636 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/data/aws_transfer_costs.csv
+-rw-r--r--   0        0        0      617 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/data/vcpu_info.csv
+-rw-r--r--   0        0        0     3078 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/exceptions.py
+-rw-r--r--   0        0        0      811 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/cert.py
+-rw-r--r--   0        0        0     4349 2023-06-22 16:57:49.416748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/chunk_store.py
+-rw-r--r--   0        0        0    15512 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_daemon.py
+-rw-r--r--   0        0        0    16570 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_daemon_api.py
+-rw-r--r--   0        0        0      718 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_onprem.py
+-rw-r--r--   0        0        0     5149 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_program.py
+-rw-r--r--   0        0        0     1732 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_queue.py
+-rw-r--r--   0        0        0        0 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/operators/__init__.py
+-rw-r--r--   0        0        0    25380 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/operators/gateway_operator.py
+-rw-r--r--   0        0        0     9658 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/operators/gateway_receiver.py
+-rw-r--r--   0        0        0       37 2023-06-22 16:58:56.452930 skyplane_nightly-0.3.2.dev20230622/skyplane/gateway_version.py
+-rw-r--r--   0        0        0    13101 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/azure_blob_interface.py
+-rw-r--r--   0        0        0     2887 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/azure_storage_account_interface.py
+-rw-r--r--   0        0        0    10871 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/cos_interface.py
+-rw-r--r--   0        0        0     2010 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/file_system_interface.py
+-rw-r--r--   0        0        0    12754 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/gcs_interface.py
+-rw-r--r--   0        0        0     5963 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/hdfs_interface.py
+-rw-r--r--   0        0        0     3287 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/object_store_interface.py
+-rw-r--r--   0        0        0     5629 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/posix_file_interface.py
+-rw-r--r--   0        0        0     3504 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/r2_interface.py
+-rw-r--r--   0        0        0    11595 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/s3_interface.py
+-rw-r--r--   0        0        0     2569 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/storage_interface.py
+-rw-r--r--   0        0        0    23237 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/planner/planner.py
+-rw-r--r--   0        0        0    18157 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/planner/solver.py
+-rw-r--r--   0        0        0     6467 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/planner/solver_ilp.py
+-rw-r--r--   0        0        0     1996 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/planner/solver_ron.py
+-rw-r--r--   0        0        0     7920 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/planner/topology.py
+-rw-r--r--   0        0        0      846 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/cache.py
+-rw-r--r--   0        0        0      617 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/definitions.py
+-rw-r--r--   0        0        0     2494 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/fn.py
+-rw-r--r--   0        0        0     1881 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/generator.py
+-rw-r--r--   0        0        0     1386 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/imports.py
+-rw-r--r--   0        0        0     2131 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/logger.py
+-rw-r--r--   0        0        0     1447 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/networking_tools.py
+-rw-r--r--   0        0        0     3162 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/path.py
+-rw-r--r--   0        0        0     1160 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/retry.py
+-rw-r--r--   0        0        0      612 2023-06-22 16:57:49.420748 skyplane_nightly-0.3.2.dev20230622/skyplane/utils/timer.py
+-rw-r--r--   0        0        0    10493 1970-01-01 00:00:00.000000 skyplane_nightly-0.3.2.dev20230622/PKG-INFO
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/LICENSE` & `skyplane_nightly-0.3.2.dev20230622/LICENSE`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/README.md` & `skyplane_nightly-0.3.2.dev20230622/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 **🔥 Blazing fast bulk data transfers between any cloud 🔥**
 
 Skyplane is a tool for blazingly fast bulk data transfers between object stores in the cloud. It provisions a fleet of VMs in the cloud to transfer data in parallel while using compression and bandwidth tiering to reduce cost.
 
 Skyplane is:
 1. 🔥 Blazing fast ([110x faster than AWS DataSync](https://skyplane.org/en/latest/benchmark.html))
 2. 🤑 Cheap (4x cheaper than rsync)
-3. 🌐 Universal (AWS, Azure and GCP)
+3. 🌐 Universal (AWS, Azure, IBM and GCP)
 
 You can use Skyplane to transfer data: 
 * between object stores within a cloud provider (e.g. AWS us-east-1 to AWS us-west-2)
 * between object stores across multiple cloud providers (e.g. AWS us-east-1 to GCP us-central1)
 * between local storage and cloud object stores (experimental)
 
 Skyplane currently supports the following source and destination endpoints (any source and destination can be combined): 
 
 | Endpoint           | Source             | Destination        |
 |--------------------|--------------------|--------------------|
 | AWS S3             | :white_check_mark: | :white_check_mark: |
 | Google Storage     | :white_check_mark: | :white_check_mark: |
 | Azure Blob Storage | :white_check_mark: | :white_check_mark: |
+| IBM Cloud Object Storage | :white_check_mark: | :white_check_mark: |
 | Local Disk         | :white_check_mark: | (in progress)      |
 
 Skyplane is an actively developed project. It will have 🔪 SHARP EDGES 🔪. Please file an issue or ask the contributors via [the #help channel on our Slack](https://join.slack.com/t/skyplaneworkspace/shared_invite/zt-1cxmedcuc-GwIXLGyHTyOYELq7KoOl6Q) if you encounter bugs.
 
 # Resources 
 - [Quickstart](#quickstart)
 - [Contributing](https://skyplane.org/en/latest/contributing.html)
@@ -43,20 +44,22 @@
 
 ## 1. Installation
 We recommend installation from PyPi:
 ```
 $ pip install "skyplane[aws]"
 
 # install support for other clouds as needed:
+
 #   $ pip install "skyplane[azure]"
 #   $ pip install "skyplane[gcp]"
+#   $ pip install "skyplane[ibmcloud]"
 #   $ pip install "skyplane[all]"
 ```
 
-Skyplane supports AWS, Azure, and GCP. You can install Skyplane with support for one or more of these clouds by specifying the corresponding extras. To install two out of three clouds, you can run `pip install "skyplane[aws,azure]"`.
+Skyplane supports AWS, Azure, IBM and GCP. You can install Skyplane with support for one or more of these clouds by specifying the corresponding extras. To install two out of three clouds, you can run `pip install "skyplane[aws,azure]"`.
 
 *GCP support on the M1 Mac*: If you are using an M1 Mac with the arm64 architecture and want to install GCP support for Skyplane, you will need to install as follows
 `GRPC_PYTHON_BUILD_SYSTEM_OPENSSL=1 GRPC_PYTHON_BUILD_SYSTEM_ZLIB=1 pip install "skyplane[aws,gcp]"`
 
 ## 2. Setup Cloud Credentials 
 
 Skyplane needs access to cloud credentials to perform transfers. To get started with setting up credentials, make sure you have cloud provider CLI tools installed:
@@ -66,25 +69,34 @@
 $ pip install awscli
 
 ---> For Google Cloud:
 $ pip install gcloud
 
 ---> For Azure:
 $ pip install azure
+
 ```
 Once you have the CLI tools setup, log into each cloud provider's CLI:
 ```
 ---> For AWS:
 $ aws configure
 
 ---> For Google Cloud:
 $ gcloud auth application-default login
 
 ---> For Azure:
 $ az login
+
+---> For IBM Cloud:
+$ Follow IBM Cloud and create an account with the resource group.
+Copy https://github.com/skyplane-project/skyplane/blob/main/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
+into `~/.bluemix/ibm_credentials` and fill your 
+IBM IAM key and credentials to your IBM Cloud object storage 
+
+
 ```
 After authenticating with each cloud provider, you can run `skyplane init` to create a configuration file for Skyplane.
 
 ```bash
 $ skyplane init
 ```
 <details>
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/pyproject.toml` & `skyplane_nightly-0.3.2.dev20230622/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "skyplane-nightly"
 packages = [{ include = "skyplane" }]
-version = "0.2.1.dev20230312"
+version = "0.3.2.dev20230622"
 description = "Skyplane efficiently transports data between cloud regions and providers."
 authors = ["Skyplane authors <skyplaneproject@gmail.com>"]
 license = "Apache-2.0"
 homepage = "https://skyplane.org/"
 repository = "https://github.com/skyplane-project/skyplane"
 documentation = "https://skyplane.org/"
 readme = "README.md"
@@ -28,47 +28,59 @@
 azure-identity = { version = ">=1.0.0", optional = true }
 azure-mgmt-authorization = { version = ">=1.0.0", optional = true }
 azure-mgmt-compute = { version = ">=24.0.0", optional = true }
 azure-mgmt-network = { version = ">=10.0.0", optional = true }
 azure-mgmt-resource = { version = ">=11.0.0", optional = true }
 azure-mgmt-storage = { version = ">=11.0.0", optional = true }
 azure-mgmt-subscription = { version = ">=1.0.0", optional = true }
+azure-mgmt-quota = { version = ">=1.1.0b3", optional = true} 
 azure-storage-blob = { version = ">=12.0.0", optional = true }
 
 # gcp dependencies
 google-api-python-client = { version = ">=2.0.2", optional = true }
 google-auth = { version = ">=2.0.0", optional = true }
 google-cloud-compute = { version = ">=1.0.0", optional = true }
 google-cloud-storage = { version = ">=1.30.0", optional = true }
+google-cloud-dataproc = { version = "^5.4.0", optional = true }
+
+# ibm dependencies 
+ibm-cloud-sdk-core = { version = ">=3.16.2", optional = true} 
+ibm-cos-sdk = { version = ">=2.12.2", optional = true} 
+ibm-cos-sdk-core = { version = ">=2.12.2", optional = true} 
+ibm-cos-sdk-s3transfer = { version = ">=2.12.2", optional = true} 
+ibm-vpc = { version = ">=0.15.0", optional = true} 
 
 # solver dependencies
-cvxpy = { version = ">=1.1.0", optional = true, extras = ["cvxopt"] }
+cvxpy = { version = ">=1.1.0", optional = true }
 graphviz = { version = ">=0.15", optional = true }
 matplotlib = { version = ">=3.0.0", optional = true }
 numpy = { version = ">=1.19.0", optional = true }
 
 # gateway dependencies
 flask = { version = "^2.1.2", optional = true }
 lz4 = { version = "^4.0.0", optional = true }
 pynacl = { version = "^1.5.0", optional = true }
 pyopenssl = { version = "^22.0.0", optional = true }
 werkzeug = { version = "^2.1.2", optional = true }
+pyarrow = "^10.0.1"
 
 [tool.poetry.extras]
 aws = ["boto3"]
-azure = ["azure-identity", "azure-mgmt-authorization", "azure-mgmt-compute", "azure-mgmt-network", "azure-mgmt-resource", "azure-mgmt-storage", "azure-mgmt-subscription", "azure-storage-blob"]
+azure = ["azure-identity", "azure-mgmt-authorization", "azure-mgmt-compute", "azure-mgmt-network", "azure-mgmt-resource", "azure-mgmt-storage", "azure-mgmt-quota", "azure-mgmt-subscription", "azure-storage-blob"]
 gcp = ["google-api-python-client", "google-auth", "google-cloud-compute", "google-cloud-storage"]
-all = ["boto3", "azure-identity", "azure-mgmt-authorization", "azure-mgmt-compute", "azure-mgmt-network", "azure-mgmt-resource", "azure-mgmt-storage", "azure-mgmt-subscription", "azure-storage-blob", "google-api-python-client", "google-auth", "google-cloud-compute", "google-cloud-storage"]
+ibm = ["ibm-cloud-sdk-core", "ibm-cos-sdk", "ibm-vpc"]
+all = ["boto3", "azure-identity", "azure-mgmt-authorization", "azure-mgmt-compute", "azure-mgmt-network", "azure-mgmt-resource", "azure-mgmt-storage", "azure-mgmt-subscription", "azure-storage-blob", "google-api-python-client", "google-auth", "google-cloud-compute", "google-cloud-storage", "ibm-cloud-sdk-core", "ibm-cos-sdk", "ibm-vpc"]
 gateway = ["flask", "lz4", "pynacl", "pyopenssl", "werkzeug"]
 solver = ["cvxpy", "graphviz", "matplotlib", "numpy"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.0"
 pytest-cov = ">=2.10.0"
 pytest-xdist = ">=2.0.0"
+black = "^23.1.0"
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 skylark = "skyplane.cli.cli:app"
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/__init__.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from pathlib import Path
 
 from skyplane import compute, exceptions
 from skyplane.api.client import SkyplaneClient
 from skyplane.api.config import TransferConfig, AWSConfig, AzureConfig, GCPConfig
 from skyplane.api.dataplane import Dataplane
+from skyplane.api.pipeline import Pipeline
 from skyplane.api.tracker import TransferHook
 
-__version__ = "0.2.1"
+__version__ = "0.3.2"
 __root__ = Path(__file__).parent.parent
 __all__ = [
     "__version__",
     "__root__",
     # modules
     "compute",
     "exceptions",
     # API
     "SkyplaneClient",
     "Dataplane",
+    "Pipeline",
     "TransferConfig",
     "AWSConfig",
     "AzureConfig",
     "GCPConfig",
     "TransferHook",
 ]
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/api/dataplane.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/api/dataplane.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from datetime import datetime
 from functools import partial
 from datetime import datetime
 
 import nacl.secret
 import nacl.utils
 import urllib3
+from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from skyplane import compute
+from skyplane.exceptions import GatewayContainerStartException
 from skyplane.api.tracker import TransferProgressTracker, TransferHook
 from skyplane.api.transfer_job import CopyJob, SyncJob, TransferJob
 from skyplane.api.config import TransferConfig
-from skyplane.planner.topology import ReplicationTopology, ReplicationTopologyGateway
+from skyplane.planner.topology import TopologyPlan, TopologyPlanGateway
 from skyplane.utils import logger
 from skyplane.utils.definitions import gateway_docker_image, tmp_log_dir
 from skyplane.utils.fn import PathLike, do_parallel
 
 if TYPE_CHECKING:
     from skyplane.api.provisioner import Provisioner
 
@@ -38,182 +40,222 @@
 
 class Dataplane:
     """A Dataplane represents a concrete Skyplane network, including topology and VMs."""
 
     def __init__(
         self,
         clientid: str,
-        topology: ReplicationTopology,
+        topology: TopologyPlan,
         provisioner: "Provisioner",
         transfer_config: TransferConfig,
+        log_dir: str,
+        debug: bool = True,
     ):
         """
         :param clientid: the uuid of the local host to create the dataplane
         :type clientid: str
         :param topology: the calculated topology during the transfer
-        :type topology: ReplicationTopology
+        :type topology: TopologyPlan
         :param provisioner: the provisioner to launch the VMs
         :type provisioner: Provisioner
         :param transfer_config: the configuration during the transfer
         :type transfer_config: TransferConfig
         """
         self.clientid = clientid
         self.topology = topology
-        self.src_region_tag = self.topology.source_region()
-        self.dst_region_tag = self.topology.sink_region()
-        regions = Counter([node.region for node in self.topology.gateway_nodes])
-        self.max_instances = int(regions[max(regions, key=regions.get)])
         self.provisioner = provisioner
         self.transfer_config = transfer_config
+        # disable for azure
+        # TODO: remove this
         self.http_pool = urllib3.PoolManager(retries=urllib3.Retry(total=3))
         self.provisioning_lock = threading.Lock()
         self.provisioned = False
+        self.log_dir = Path(log_dir)
         self.transfer_dir = tmp_log_dir / "transfer_logs" / datetime.now().strftime("%Y%m%d_%H%M%S")
         self.transfer_dir.mkdir(exist_ok=True, parents=True)
 
         # transfer logs
         self.transfer_dir = tmp_log_dir / "transfer_logs" / datetime.now().strftime("%Y%m%d_%H%M%S")
         self.transfer_dir.mkdir(exist_ok=True, parents=True)
+        self.debug = debug
 
         # pending tracker tasks
-        self.jobs_to_dispatch: List[TransferJob] = []
         self.pending_transfers: List[TransferProgressTracker] = []
-        self.bound_nodes: Dict[ReplicationTopologyGateway, compute.Server] = {}
+        self.bound_nodes: Dict[TopologyPlanGateway, compute.Server] = {}
+
+    def _start_gateway(
+        self,
+        gateway_docker_image: str,
+        gateway_node: TopologyPlanGateway,
+        gateway_server: compute.Server,
+        gateway_log_dir: Optional[PathLike],
+        authorize_ssh_pub_key: Optional[str] = None,
+        e2ee_key_bytes: Optional[str] = None,
+    ):
+        # map outgoing ports
+        setup_args = {}
+        for gateway_id, n_conn in self.topology.get_outgoing_paths(gateway_node.gateway_id).items():
+            node = self.topology.get_gateway(gateway_id)
+            # use private ips for gcp to gcp connection
+            src_provider, dst_provider = gateway_node.region.split(":")[0], node.region.split(":")[0]
+            if src_provider == dst_provider and src_provider == "gcp":
+                setup_args[self.bound_nodes[node].private_ip()] = n_conn
+            else:
+                setup_args[self.bound_nodes[node].public_ip()] = n_conn
+        logger.fs.debug(f"[Dataplane._start_gateway] Setup args for {gateway_node}: {setup_args}")
+
+        if gateway_log_dir:
+            gateway_server.init_log_files(gateway_log_dir)
+        if authorize_ssh_pub_key:
+            gateway_server.copy_public_key(authorize_ssh_pub_key)
+
+        # write gateway programs
+        gateway_program_filename = Path(f"{gateway_log_dir}/gateway_program_{gateway_node.gateway_id}.json")
+        with open(gateway_program_filename, "w") as f:
+            f.write(gateway_node.gateway_program.to_json())
+
+        # start gateway
+        gateway_server.start_gateway(
+            # setup_args,
+            gateway_docker_image=gateway_docker_image,
+            gateway_program_path=str(gateway_program_filename),
+            gateway_info_path=f"{gateway_log_dir}/gateway_info.json",
+            e2ee_key_bytes=None,  # TODO: remove
+            use_bbr=self.transfer_config.use_bbr,  # TODO: remove
+            use_compression=self.transfer_config.use_compression,
+            use_socket_tls=self.transfer_config.use_socket_tls,
+        )
 
     def provision(
         self,
         allow_firewall: bool = True,
         gateway_docker_image: str = os.environ.get("SKYPLANE_DOCKER_IMAGE", gateway_docker_image()),
-        gateway_log_dir: Optional[PathLike] = None,
         authorize_ssh_pub_key: Optional[str] = None,
         max_jobs: int = 16,
         spinner: bool = False,
     ):
         """
         Provision the transfer gateways.
 
         :param allow_firewall: whether to apply firewall rules in the gatweway network (default: True)
         :type allow_firewall: bool
         :param gateway_docker_image: Docker image token in github
         :type gateway_docker_image: str
-        :param gateway_log_dir: path to the log directory in the remote gatweways
-        :type gateway_log_dir: PathLike
         :param authorize_ssh_pub_key: authorization ssh key to the remote gateways
         :type authorize_ssh_pub_key: str
         :param max_jobs: maximum number of provision jobs to launch concurrently (default: 16)
         :type max_jobs: int
-        :param spinner: whether to show the spinner during the job (default: False)
+        :param spinner: whether to show the spinner during the job (default: False)its to determine how many instances to create in each region
         :type spinner: bool
         """
+        # TODO: support on-sided transfers but not requiring VMs to be created in source/destination regions
         with self.provisioning_lock:
             if self.provisioned:
                 logger.error("Cannot provision dataplane, already provisioned!")
                 return
-            is_aws_used = any(n.region.startswith("aws:") for n in self.topology.nodes)
-            is_azure_used = any(n.region.startswith("azure:") for n in self.topology.nodes)
-            is_gcp_used = any(n.region.startswith("gcp:") for n in self.topology.nodes)
+            is_aws_used = any(n.region_tag.startswith("aws:") for n in self.topology.get_gateways())
+            is_azure_used = any(n.region_tag.startswith("azure:") for n in self.topology.get_gateways())
+            is_gcp_used = any(n.region_tag.startswith("gcp:") for n in self.topology.get_gateways())
+            is_ibmcloud_used = any(n.region_tag.startswith("ibmcloud:") for n in self.topology.get_gateways())
 
             # create VMs from the topology
-            for node in self.topology.gateway_nodes:
-                cloud_provider, region = node.region.split(":")
+            for node in self.topology.get_gateways():
+                cloud_provider, region = node.region_tag.split(":")
+                assert (
+                    cloud_provider != "cloudflare"
+                ), f"Cannot create VMs in certain cloud providers: check planner output {self.topology.to_dict()}"
                 self.provisioner.add_task(
                     cloud_provider=cloud_provider,
                     region=region,
-                    vm_type=getattr(self.transfer_config, f"{cloud_provider}_instance_class"),
+                    vm_type=node.vm_type or getattr(self.transfer_config, f"{cloud_provider}_instance_class"),
                     spot=getattr(self.transfer_config, f"{cloud_provider}_use_spot_instances"),
                     autoterminate_minutes=self.transfer_config.autoterminate_minutes,
                 )
 
             # initialize clouds
-            self.provisioner.init_global(aws=is_aws_used, azure=is_azure_used, gcp=is_gcp_used)
+            self.provisioner.init_global(aws=is_aws_used, azure=is_azure_used, gcp=is_gcp_used, ibmcloud=is_ibmcloud_used)
 
             # provision VMs
             uuids = self.provisioner.provision(
                 authorize_firewall=allow_firewall,
                 max_jobs=max_jobs,
                 spinner=spinner,
             )
 
             # bind VMs to nodes
             servers = [self.provisioner.get_node(u) for u in uuids]
             servers_by_region = defaultdict(list)
             for s in servers:
                 servers_by_region[s.region_tag].append(s)
-            for node in self.topology.gateway_nodes:
-                instance = servers_by_region[node.region].pop()
+            for node in self.topology.get_gateways():
+                instance = servers_by_region[node.region_tag].pop()
                 self.bound_nodes[node] = instance
+
+                # set ip addresses (for gateway program generation)
+                self.topology.set_ip_addresses(node.gateway_id, self.bound_nodes[node].private_ip(), self.bound_nodes[node].public_ip())
+
             logger.fs.debug(f"[Dataplane.provision] bound_nodes = {self.bound_nodes}")
             gateway_bound_nodes = self.bound_nodes.copy()
 
             # start gateways
             self.provisioned = True
 
-        def _start_gateway(
-            gateway_node: ReplicationTopologyGateway,
-            gateway_server: compute.Server,
-        ):
-            # map outgoing ports
-            setup_args = {}
-            for n, v in self.topology.get_outgoing_paths(gateway_node).items():
-                if isinstance(n, ReplicationTopologyGateway):
-                    # use private ips for gcp to gcp connection
-                    src_provider, dst_provider = gateway_node.region.split(":")[0], n.region.split(":")[0]
-                    if src_provider == dst_provider and src_provider == "gcp":
-                        setup_args[self.bound_nodes[n].private_ip()] = v
-                    else:
-                        setup_args[self.bound_nodes[n].public_ip()] = v
-            am_source = gateway_node in self.topology.source_instances()
-            am_sink = gateway_node in self.topology.sink_instances()
-            logger.fs.debug(f"[Dataplane._start_gateway] Setup args for {gateway_node}: {setup_args}")
-
-            # start gateway
-            if gateway_log_dir:
-                gateway_server.init_log_files(gateway_log_dir)
-            if authorize_ssh_pub_key:
-                gateway_server.copy_public_key(authorize_ssh_pub_key)
-            gateway_server.start_gateway(
-                setup_args,
-                gateway_docker_image=gateway_docker_image,
-                e2ee_key_bytes=e2ee_key_bytes if (self.transfer_config.use_e2ee and (am_source or am_sink)) else None,
-                use_bbr=self.transfer_config.use_bbr,
-                use_compression=self.transfer_config.use_compression,
-                use_socket_tls=self.transfer_config.use_socket_tls,
-            )
-
         # todo: move server.py:start_gateway here
         logger.fs.info(f"Using docker image {gateway_docker_image}")
         e2ee_key_bytes = nacl.utils.random(nacl.secret.SecretBox.KEY_SIZE)
 
+        # create gateway logging dir
+        gateway_program_dir = f"{self.log_dir}/programs"
+        Path(gateway_program_dir).mkdir(exist_ok=True, parents=True)
+        logger.fs.info(f"Writing gateway programs to {gateway_program_dir}")
+
+        # write gateway info file
+        gateway_info_path = f"{gateway_program_dir}/gateway_info.json"
+        with open(gateway_info_path, "w") as f:
+            json.dump(self.topology.get_gateway_info_json(), f, indent=4)
+        logger.fs.info(f"Writing gateway info to {gateway_info_path}")
+
+        # start gateways in parallel
         jobs = []
         for node, server in gateway_bound_nodes.items():
-            jobs.append(partial(_start_gateway, node, server))
+            jobs.append(
+                partial(self._start_gateway, gateway_docker_image, node, server, gateway_program_dir, authorize_ssh_pub_key, e2ee_key_bytes)
+            )
         logger.fs.debug(f"[Dataplane.provision] Starting gateways on {len(jobs)} servers")
-        do_parallel(lambda fn: fn(), jobs, n=-1, spinner=spinner, spinner_persist=spinner, desc="Starting gateway container on VMs")
+        try:
+            do_parallel(lambda fn: fn(), jobs, n=-1, spinner=spinner, spinner_persist=spinner, desc="Starting gateway container on VMs")
+        except Exception as e:
+            self.copy_gateway_logs()
+            raise GatewayContainerStartException(f"Error starting gateways. Please check gateway logs {self.transfer_dir}")
 
     def copy_gateway_logs(self):
         # copy logs from all gateways in parallel
         def copy_log(instance):
+            out_file = self.transfer_dir / f"gateway_{instance.uuid()}.stdout"
+            err_file = self.transfer_dir / f"gateway_{instance.uuid()}.stderr"
+            logger.fs.info(f"[Dataplane.copy_gateway_logs] Copying logs from {instance.uuid()}: {out_file}")
             instance.run_command("sudo docker logs -t skyplane_gateway 2> /tmp/gateway.stderr > /tmp/gateway.stdout")
-            instance.download_file("/tmp/gateway.stdout", self.transfer_dir / f"gateway_{instance.uuid()}.stdout")
-            instance.download_file("/tmp/gateway.stderr", self.transfer_dir / f"gateway_{instance.uuid()}.stderr")
+            instance.download_file("/tmp/gateway.stdout", out_file)
+            instance.download_file("/tmp/gateway.stderr", err_file)
 
+        print("COPY GATEWAY LOGS")
         do_parallel(copy_log, self.bound_nodes.values(), n=-1)
 
-    def deprovision(self, max_jobs: int = 64, spinner: bool = False, debug: bool = False):
+    def deprovision(self, max_jobs: int = 64, spinner: bool = False):
         """
         Deprovision the remote gateways
 
         :param max_jobs: maximum number of jobs to deprovision the remote gateways (default: 64)
         :type max_jobs: int
         :param spinner: Whether to show the spinner during the job (default: False)
         :type spinner: bool
         """
         with self.provisioning_lock:
-            if debug:
-                logger.fs.info("Copying gateway logs to {self.transfer_dir}")
+            if self.debug and self.provisioned:
+                logger.fs.info(f"Copying gateway logs to {self.transfer_dir}")
                 self.copy_gateway_logs()
 
             if not self.provisioned:
                 logger.fs.warning("Attempting to deprovision dataplane that is not provisioned, this may be from auto_deprovision.")
             # wait for tracker tasks
             try:
                 for task in self.pending_transfers:
@@ -236,95 +278,51 @@
             _, instance = args
             reply = self.http_pool.request("GET", f"{instance.gateway_api_url}/api/v1/errors")
             if reply.status != 200:
                 raise Exception(f"Failed to get error logs from gateway instance {instance.instance_name()}: {reply.data.decode('utf-8')}")
             return json.loads(reply.data.decode("utf-8"))["errors"]
 
         errors: Dict[str, List[str]] = {}
-        for (_, instance), result in do_parallel(get_error_logs, self.bound_nodes.items(), n=-1):
+        for (_, instance), result in do_parallel(get_error_logs, self.bound_nodes.items(), n=8):
             errors[instance] = result
         return errors
 
     def auto_deprovision(self) -> DataplaneAutoDeprovision:
         """Returns a context manager that will automatically call deprovision upon exit."""
         return DataplaneAutoDeprovision(self)
 
     def source_gateways(self) -> List[compute.Server]:
         """Returns a list of source gateway nodes"""
         return [self.bound_nodes[n] for n in self.topology.source_instances()] if self.provisioned else []
 
-    def sink_gateways(self) -> List[compute.Server]:
+    def sink_gateways(self, region_tag: Optional[str] = None) -> Dict[str, List[compute.Server]]:
         """Returns a list of sink gateway nodes"""
-        return [self.bound_nodes[n] for n in self.topology.sink_instances()] if self.provisioned else []
-
-    def copy_log(self, instance):
-        instance.run_command("sudo docker logs -t skyplane_gateway 2> /tmp/gateway.stderr > /tmp/gateway.stdout")
-        instance.download_file("/tmp/gateway.stdout", self.transfer_dir / f"gateway_{instance.uuid()}.stdout")
-        instance.download_file("/tmp/gateway.stderr", self.transfer_dir / f"gateway_{instance.uuid()}.stderr")
-
-    def queue_copy(
-        self,
-        src: str,
-        dst: str,
-        recursive: bool = False,
-    ) -> str:
-        """
-        Add a copy job to job list.
-        Return the uuid of the job.
-
-        :param src: source prefix to copy from
-        :type src: str
-        :param dst: the destination of the transfer
-        :type dst: str
-        :param recursive: if true, will copy objects at folder prefix recursively (default: False)
-        :type recursive: bool
-        """
-        job = CopyJob(src, dst, recursive, requester_pays=self.transfer_config.requester_pays)
-        logger.fs.debug(f"[SkyplaneClient] Queued copy job {job}")
-        self.jobs_to_dispatch.append(job)
-        return job.uuid
-
-    def queue_sync(
-        self,
-        src: str,
-        dst: str,
-    ) -> str:
-        """
-        Add a sync job to job list.
-        Return the uuid of the job.
-
-        :param src: Source prefix to copy from
-        :type src: str
-        :param dst: The destination of the transfer
-        :type dst: str
-        :param recursive: If true, will copy objects at folder prefix recursively (default: False)
-        :type recursive: bool
-        """
-        job = SyncJob(src, dst, recursive=True, requester_pays=self.transfer_config.requester_pays)
-        logger.fs.debug(f"[SkyplaneClient] Queued sync job {job}")
-        self.jobs_to_dispatch.append(job)
-        return job.uuid
+        return (
+            {region: [self.bound_nodes[n] for n in nodes] for region, nodes in self.topology.sink_instances(region_tag).items()}
+            if self.provisioned
+            else {}
+        )
 
-    def run_async(self, hooks: Optional[TransferHook] = None) -> TransferProgressTracker:
+    def run_async(self, jobs: List[TransferJob], hooks: Optional[TransferHook] = None) -> TransferProgressTracker:
         """Start the transfer asynchronously. The main thread will not be blocked.
 
         :param hooks: Tracks the status of the transfer
         :type hooks: TransferHook
         """
         if not self.provisioned:
             logger.error("Dataplane must be pre-provisioned. Call dataplane.provision() before starting a transfer")
-        tracker = TransferProgressTracker(self, self.jobs_to_dispatch, self.transfer_config, hooks)
+        print("discord", jobs)
+        tracker = TransferProgressTracker(self, jobs, self.transfer_config, hooks)
         self.pending_transfers.append(tracker)
         tracker.start()
-        logger.fs.info(f"[SkyplaneClient] Started async transfer with {len(self.jobs_to_dispatch)} jobs")
-        self.jobs_to_dispatch = []
+        logger.fs.info(f"[SkyplaneClient] Started async transfer with {len(jobs)} jobs")
         return tracker
 
-    def run(self, hooks: Optional[TransferHook] = None):
+    def run(self, jobs: List[TransferJob], hooks: Optional[TransferHook] = None):
         """Start the transfer in the main thread. Wait until the transfer is complete.
 
         :param hooks: Tracks the status of the transfer
         :type hooks: TransferHook
         """
-        tracker = self.run_async(hooks)
+        tracker = self.run_async(jobs, hooks)
         logger.fs.debug(f"[SkyplaneClient] Waiting for transfer to complete")
         tracker.join()
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/api/provisioner.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/api/provisioner.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,64 +47,74 @@
 
     def __init__(
         self,
         aws_auth: Optional[compute.AWSAuthentication] = None,
         azure_auth: Optional[compute.AzureAuthentication] = None,
         gcp_auth: Optional[compute.GCPAuthentication] = None,
         host_uuid: Optional[str] = None,
+        ibmcloud_auth: Optional[compute.IBMCloudAuthentication] = None,
     ):
         """
         :param aws_auth: authentication information for aws
         :type aws_auth: compute.AWSAuthentication
         :param azure_auth: authentication information for azure
         :type azure_auth: compute.AzureAuthentication
         :param gcp_auth: authentication information for gcp
         :type gcp_auth: compute.GCPAuthentication
         :param host_uuid: the uuid of the local host that requests the provision task
         :type host_uuid: string
+        :param ibmcloud_auth: authentication information for aws
+        :type ibmcloud_auth: compute.IBMCloudAuthentication
         """
         self.aws_auth = aws_auth
         self.azure_auth = azure_auth
         self.gcp_auth = gcp_auth
         self.host_uuid = host_uuid
+        self.ibmcloud_auth = ibmcloud_auth
         self._make_cloud_providers()
         self.temp_nodes: Set[compute.Server] = set()  # temporary area to store nodes that should be terminated upon exit
         self.pending_provisioner_tasks: List[ProvisionerTask] = []
         self.provisioned_vms: Dict[str, compute.Server] = {}
 
         # store GCP firewall rules to be deleted upon exit
         self.gcp_firewall_rules: Set[str] = set()
 
     def _make_cloud_providers(self):
         self.aws = compute.AWSCloudProvider(
             key_prefix=f"skyplane{'-'+self.host_uuid.replace('-', '') if self.host_uuid else ''}", auth=self.aws_auth
         )
         self.azure = compute.AzureCloudProvider(auth=self.azure_auth)
         self.gcp = compute.GCPCloudProvider(auth=self.gcp_auth)
+        self.ibmcloud = compute.IBMCloudProvider(auth=self.ibmcloud_auth)
 
-    def init_global(self, aws: bool = True, azure: bool = True, gcp: bool = True):
+    def init_global(self, aws: bool = True, azure: bool = True, gcp: bool = True, ibmcloud: bool = True):
         """
         Initialize the global cloud providers by configuring with credentials
 
         :param aws: whether to configure aws (default: True)
         :type aws: bool
         :param azure: whether to configure azure (default: True)
         :type azure: bool
         :param gcp: whether to configure gcp (default: True)
         :type gcp: bool
+        :param ibmcloud: whether to configure ibmcloud (default: True)
+        :type ibmcloud: bool
         """
         logger.fs.info(f"[Provisioner.init_global] Initializing global resources for aws={aws}, azure={azure}, gcp={gcp}")
         jobs = []
         if aws:
             jobs.append(partial(self.aws.setup_global, attach_policy_arn="arn:aws:iam::aws:policy/AmazonS3FullAccess"))
         if azure:
             jobs.append(self.azure.create_ssh_key)
             jobs.append(self.azure.set_up_resource_group)
         if gcp:
             jobs.append(self.gcp.setup_global)
+        if ibmcloud:
+            jobs.append(self.ibmcloud.setup_global)
+
         do_parallel(lambda fn: fn(), jobs, spinner=False)
 
     def add_task(
         self,
         cloud_provider: str,
         region: str,
         vm_type: str,
@@ -150,22 +160,24 @@
                 assert self.aws.auth.enabled(), "AWS credentials not configured"
                 server = self.aws.provision_instance(task.region, task.vm_type, use_spot_instances=task.spot, tags=task.tags)
             elif task.cloud_provider == "azure":
                 assert self.azure.auth.enabled(), "Azure credentials not configured"
                 server = self.azure.provision_instance(task.region, task.vm_type, use_spot_instances=task.spot, tags=task.tags)
             elif task.cloud_provider == "gcp":
                 assert self.gcp.auth.enabled(), "GCP credentials not configured"
-                # todo specify network tier in ReplicationTopology
                 server = self.gcp.provision_instance(
                     task.region,
                     task.vm_type,
                     use_spot_instances=task.spot,
                     gcp_premium_network=False,
                     tags=task.tags,
                 )
+            elif task.cloud_provider == "ibmcloud":
+                assert self.ibmcloud.auth.enabled(), "IBM Cloud credentials not configured"
+                server = self.ibmcloud.provision_instance(task.region, task.vm_type, tags=task.tags)
             else:
                 raise NotImplementedError(f"Unknown provider {task.cloud_provider}")
         logger.fs.debug(f"[Provisioner._provision_task] Provisioned {server} in {t.elapsed:.2f}s")
         self.temp_nodes.add(server)
         self.provisioned_vms[task.uuid] = server
         server.wait_for_ssh_ready()
         if task.autoterminate_minutes:
@@ -186,24 +198,36 @@
         if not self.pending_provisioner_tasks:
             return []
 
         # copy list to avoid concurrency issue
         provision_tasks = list(self.pending_provisioner_tasks)
         aws_provisioned = any([task.cloud_provider == "aws" for task in provision_tasks])
         aws_regions = set([task.region for task in provision_tasks if task.cloud_provider == "aws"])
+        ibmcloud_regions = set([task.region for task in provision_tasks if task.cloud_provider == "ibmcloud"])
         azure_provisioned = any([task.cloud_provider == "azure" for task in provision_tasks])
         gcp_provisioned = any([task.cloud_provider == "gcp" for task in provision_tasks])
+        ibmcloud_provisioned = any([task.cloud_provider == "ibmcloud" for task in provision_tasks])
 
         # configure regions
         if aws_provisioned:
             do_parallel(
                 self.aws.setup_region, list(set(aws_regions)), spinner=spinner, spinner_persist=False, desc="Configuring AWS regions"
             )
             logger.fs.info(f"[Provisioner.provision] Configured AWS regions {aws_regions}")
 
+        if ibmcloud_provisioned:
+            do_parallel(
+                self.ibmcloud.setup_region,
+                list(set(ibmcloud_regions)),
+                spinner=spinner,
+                spinner_persist=False,
+                desc="Configuring IBM Cloud regions",
+            )
+            logger.fs.info(f"[Provisioner.provision] Configured IBM Cloud regions {ibmcloud_regions}")
+
         # provision VMs
         logger.fs.info(f"[Provisioner.provision] Provisioning {len(provision_tasks)} VMs")
         results: List[Tuple[ProvisionerTask, compute.Server]] = do_parallel(
             self._provision_task,
             provision_tasks,
             n=max_jobs,
             spinner=spinner,
@@ -212,17 +236,21 @@
         )
 
         # configure firewall
         if authorize_firewall:
             public_ips = [s.public_ip() for _, s in results]
             # authorize access to private IPs for GCP VMs due to global VPC
             private_ips = [s.private_ip() for t, s in results if t.cloud_provider == "gcp"]
+
             authorize_ip_jobs = []
+            if ibmcloud_provisioned:
+                authorize_ip_jobs.extend([partial(self.ibmcloud.add_ips_to_security_group, r, public_ips) for r in set(ibmcloud_regions)])
+            # NOTE: the following setup is for broadcast only
             if aws_provisioned:
-                authorize_ip_jobs.extend([partial(self.aws.add_ips_to_security_group, r, public_ips) for r in set(aws_regions)])
+                authorize_ip_jobs.extend([partial(self.aws.add_ips_to_security_group, r, None) for r in set(aws_regions)])
             if gcp_provisioned:
 
                 def authorize_gcp_gateways():
                     self.gcp_firewall_rules.add(self.gcp.authorize_gateways(public_ips + private_ips))
 
                 authorize_ip_jobs.append(authorize_gcp_gateways)
 
@@ -270,14 +298,15 @@
                 self.temp_nodes.remove(server)
             logger.fs.info(f"[Provisioner.deprovision] Terminated {server}")
 
         servers = list(self.provisioned_vms.values()) + list(self.temp_nodes)
         aws_deprovisioned = any([s.provider == "aws" for s in servers])
         azure_deprovisioned = any([s.provider == "azure" for s in servers])
         gcp_deprovisioned = any([s.provider == "gcp" for s in servers])
+        ibmcloud_deprovisioned = any([s.provider == "ibmcloud" for s in servers])
         if azure_deprovisioned:
             logger.warning("Azure deprovisioning is very slow. Please be patient.")
         logger.fs.info(f"[Provisioner.deprovision] Deprovisioning {len(servers)} VMs")
         do_parallel(
             deprovision_gateway_instance,
             servers,
             n=max_jobs,
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/api/transfer_job.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/api/transfer_job.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,199 @@
 import json
+import time
+import time
+import typer
 import math
 import queue
 import sys
 import threading
 import time
 import uuid
 from abc import ABC
 from collections import defaultdict
 from dataclasses import dataclass, field
 from queue import Queue
-from typing import TYPE_CHECKING, Callable, Generator, List, Optional, Tuple, TypeVar
+
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Callable, Generator, List, Optional, Tuple, TypeVar, Dict
+
+from abc import ABC, abstractmethod
 
 import urllib3
 from rich import print as rprint
+from functools import partial
 
 from skyplane import exceptions
 from skyplane.api.config import TransferConfig
 from skyplane.chunk import Chunk, ChunkRequest
-from skyplane.obj_store.azure_blob_interface import AzureBlobObject
+from skyplane.obj_store.azure_blob_interface import AzureBlobInterface, AzureBlobObject
 from skyplane.obj_store.gcs_interface import GCSObject
-from skyplane.obj_store.object_store_interface import ObjectStoreInterface, ObjectStoreObject
+from skyplane.obj_store.r2_interface import R2Object
+from skyplane.obj_store.storage_interface import StorageInterface
+from skyplane.obj_store.object_store_interface import ObjectStoreObject, ObjectStoreInterface
 from skyplane.obj_store.s3_interface import S3Object
 from skyplane.utils import logger
 from skyplane.utils.definitions import MB
 from skyplane.utils.fn import do_parallel
 from skyplane.utils.path import parse_path
+from skyplane.utils.retry import retry_backoff
 
 if TYPE_CHECKING:
     from skyplane.api.dataplane import Dataplane
 
 T = TypeVar("T")
 
 
+@dataclass
+class TransferPair:
+    "Represents transfer pair between source and destination"
+
+    def __init__(self, src_obj: ObjectStoreObject, dst_objs: Dict[str, ObjectStoreObject], dst_key: str):
+        self.src_obj = src_obj
+        self.dst_objs = dst_objs
+        self.dst_key = dst_key  # shared destination key across all chunks (differnt prefixes)
+
+
+@dataclass
+class GatewayMessage:
+    def __init__(self, chunk: Optional[Chunk] = None, upload_id_mapping: Optional[Dict[str, Tuple[str, str]]] = None):
+        self.chunk = chunk
+        # TODO: currently, the mapping ID is per-region, however this should be per-bucket, as there may be multiple
+        # target buckets in the same region
+        self.upload_id_mapping = upload_id_mapping  # region_tag: (upload_id, dst_key)
+
+
 class Chunker:
     """class that chunks the original files and makes the chunk requests"""
 
     def __init__(
         self,
-        src_iface: ObjectStoreInterface,
-        dst_iface: ObjectStoreInterface,
+        src_iface: StorageInterface,
+        dst_ifaces: List[StorageInterface],
         transfer_config: TransferConfig,
-        concurrent_multipart_chunk_threads: int = 64,
+        concurrent_multipart_chunk_threads: Optional[int] = 64,
+        num_partitions: Optional[int] = 1,
     ):
         """
         :param src_iface: source object store interface
-        :type src_iface: ObjectStoreInterface
+        :type src_iface: StorageInterface
         :param dst_iface: destination object store interface
-        :type dst_iface: ObjectStoreInterface
+        :type dst_ifaces: List[StorageInterface]
         :param transfer_config: the configuration during the transfer
         :type transfer_config: TransferConfig
         :param concurrent_multipart_chunk_threads: the maximum number of concurrent threads that dispatch multipart chunk requests (default: 64)
         :type concurrent_multipart_chunk_threads: int
         """
         self.src_iface = src_iface
-        self.dst_iface = dst_iface
+        self.dst_ifaces = dst_ifaces
         self.transfer_config = transfer_config
         self.multipart_upload_requests = []
         self.concurrent_multipart_chunk_threads = concurrent_multipart_chunk_threads
+        self.num_partitions = num_partitions
 
     def _run_multipart_chunk_thread(
         self,
         exit_event: threading.Event,
-        in_queue: "Queue[Tuple[ObjectStoreObject, ObjectStoreObject]]",
-        out_queue: "Queue[Chunk]",
+        in_queue: "Queue[TransferPair]",
+        out_queue_chunks: "Queue[GatewayMessage]",
     ):
         """Chunks large files into many small chunks."""
-        region = self.dst_iface.region_tag()
-        bucket = self.dst_iface.bucket()
         while not exit_event.is_set():
             try:
-                input_data = in_queue.get(block=False, timeout=0.1)
+                transfer_pair = in_queue.get(block=False, timeout=0.1)
             except queue.Empty:
                 continue
 
-            # get source and destination object and then compute number of chunks
-            src_object, dest_object = input_data
-            mime_type = self.src_iface.get_obj_mime_type(src_object.key)
-            upload_id = self.dst_iface.initiate_multipart_upload(dest_object.key, mime_type=mime_type)
-            chunk_size_bytes = int(self.transfer_config.multipart_chunk_size_mb * MB)
-            num_chunks = math.ceil(src_object.size / chunk_size_bytes)
-            if num_chunks > self.transfer_config.multipart_max_chunks:
-                chunk_size_bytes = int(src_object.size / self.transfer_config.multipart_max_chunks)
-                chunk_size_bytes = math.ceil(chunk_size_bytes / MB) * MB  # round to next largest mb
-                num_chunks = math.ceil(src_object.size / chunk_size_bytes)
+            src_object = transfer_pair.src_obj
+            dest_objects = transfer_pair.dst_objs
+            dest_key = transfer_pair.dst_key
+            if isinstance(self.src_iface, ObjectStoreInterface):
+                mime_type = self.src_iface.get_obj_mime_type(src_object.key)
+                # create multipart upload request per destination
+                upload_id_mapping = {}
+                for dest_iface in self.dst_ifaces:
+                    dest_object = dest_objects[dest_iface.region_tag()]
+                    upload_id = dest_iface.initiate_multipart_upload(dest_object.key, mime_type=mime_type)
+                    # print(f"Created upload id for key {dest_object.key} with upload id {upload_id} for bucket {dest_iface.bucket_name}")
+                    # store mapping between key and upload id for each region
+                    upload_id_mapping[dest_iface.region_tag()] = (src_object.key, upload_id)
+                out_queue_chunks.put(GatewayMessage(upload_id_mapping=upload_id_mapping))  # send to output queue
 
-            assert num_chunks * chunk_size_bytes >= src_object.size
-            # create chunks
-            offset = 0
-            part_num = 1
-            parts = []
-            for _ in range(num_chunks):
-                file_size_bytes = min(chunk_size_bytes, src_object.size - offset)
-                assert file_size_bytes > 0, f"file size <= 0 {file_size_bytes}"
-                chunk = Chunk(
-                    src_key=src_object.key,
-                    dest_key=dest_object.key,
-                    chunk_id=uuid.uuid4().hex,
-                    file_offset_bytes=offset,
-                    chunk_length_bytes=file_size_bytes,
-                    part_number=part_num,
-                    upload_id=upload_id,
-                )
-                offset += file_size_bytes
-                parts.append(part_num)
-                part_num += 1
-                out_queue.put(chunk)
-
-            self.multipart_upload_requests.append(dict(upload_id=upload_id, key=dest_object.key, parts=parts, region=region, bucket=bucket))
+                # get source and destination object and then compute number of chunks
+                chunk_size_bytes = int(self.transfer_config.multipart_chunk_size_mb * MB)
+                num_chunks = math.ceil(src_object.size / chunk_size_bytes)
+                if num_chunks > self.transfer_config.multipart_max_chunks:
+                    chunk_size_bytes = int(src_object.size / self.transfer_config.multipart_max_chunks)
+                    chunk_size_bytes = math.ceil(chunk_size_bytes / MB) * MB  # round to next largest mb
+                    num_chunks = math.ceil(src_object.size / chunk_size_bytes)
+
+                assert num_chunks * chunk_size_bytes >= src_object.size
+                # create chunks
+                offset = 0
+                part_num = 1
+                parts = []
+                for _ in range(num_chunks):
+                    file_size_bytes = min(chunk_size_bytes, src_object.size - offset)
+                    assert file_size_bytes > 0, f"file size <= 0 {file_size_bytes}"
+                    chunk = Chunk(
+                        src_key=src_object.key,
+                        dest_key=dest_key,  # dest_object.key, # TODO: upload basename (no prefix)
+                        chunk_id=uuid.uuid4().hex,
+                        file_offset_bytes=offset,
+                        partition_id=str(part_num % self.num_partitions),
+                        chunk_length_bytes=file_size_bytes,
+                        part_number=part_num,
+                        # upload_id=upload_id,
+                        multi_part=True,
+                    )
+                    assert upload_id is not None, f"Upload id cannot be None for multipart upload for {src_object.key}"
+                    assert part_num is not None, f"Partition cannot be none {part_num}"
+                    offset += file_size_bytes
+                    parts.append(part_num)
+                    part_num += 1
+                    out_queue_chunks.put(GatewayMessage(chunk=chunk))
+
+                # store multipart ids
+                for dest_iface in self.dst_ifaces:
+                    bucket = dest_iface.bucket()
+                    region = dest_iface.region_tag()
+                    dest_object = dest_objects[region]
+                    _, upload_id = upload_id_mapping[region]
+
+                    metadata = None
+                    # Convert parts to base64 and store mime_type if destination interface is AzureBlobInterface
+                    if isinstance(dest_iface, AzureBlobInterface):
+                        block_ids = list(map(lambda part_num: AzureBlobInterface.id_to_base64_encoding(part_num, dest_object.key), parts))
+                        metadata = (block_ids, mime_type)
+
+                    self.multipart_upload_requests.append(
+                        dict(upload_id=upload_id, key=dest_object.key, parts=parts, region=region, bucket=bucket, metadata=metadata)
+                    )
+            else:
+                mime_type = None
+                raise NotImplementedError("Multipart not implement for non-object store interfaces")
 
-    def to_chunk_requests(self, gen_in: Generator[Chunk, None, None]) -> Generator[ChunkRequest, None, None]:
-        """Converts a generator of chunks to a generator of chunk requests.
+    # def to_chunk_requests(self, gen_in: Generator[Chunk, None, None]) -> Generator[ChunkRequest, None, None]:
+    #    """Converts a generator of chunks to a generator of chunk requests.
 
-        :param gen_in: generator that generates chunk requests
-        :type gen_in: Generator
-        """
-        src_region = self.src_iface.region_tag()
-        dest_region = self.dst_iface.region_tag()
-        src_bucket = self.src_iface.bucket()
-        dest_bucket = self.dst_iface.bucket()
-        for chunk in gen_in:
-            yield ChunkRequest(
-                chunk=chunk,
-                src_region=src_region,
-                dst_region=dest_region,
-                src_object_store_bucket=src_bucket,
-                dst_object_store_bucket=dest_bucket,
-                src_type="object_store",
-                dst_type="object_store",
-            )
+    #    :param gen_in: generator that generates chunk requests
+    #    :type gen_in: Generator
+    #    """
+    #    src_region = self.src_iface.region_tag()
+    #    src_bucket = self.src_iface.bucket()
+    #    for chunk in gen_in:
+    #        yield ChunkRequest(
+    #            chunk=chunk,
+    #            src_region=src_region,
+    #            #dst_region=dest_region,
+    #            src_object_store_bucket=src_bucket,
+    #            #dst_object_store_bucket=dest_bucket,
+    #            src_type="object_store",
+    #            #dst_type="object_store",
+    #        )
 
     @staticmethod
     def map_object_key_prefix(source_prefix: str, source_key: str, dest_prefix: str, recursive: bool = False):
         """
         map_object_key_prefix computes the mapping of a source key in a bucket prefix to the destination.
         Users invoke a transfer via the CLI; aws s3 cp s3://bucket/source_prefix s3://bucket/dest_prefix.
         The CLI will query the object store for all objects in the source prefix and map them to the
@@ -179,104 +241,145 @@
                     src_path_after_prefix = source_key[len(source_prefix) :]
                     src_path_after_prefix = src_path_after_prefix[1:] if src_path_after_prefix.startswith("/") else src_path_after_prefix
                     return join(dest_prefix, src_path_after_prefix)
 
     def transfer_pair_generator(
         self,
         src_prefix: str,
-        dst_prefix: str,
+        dst_prefixes: List[str],
         recursive: bool,
-        prefilter_fn: Optional[Callable[[ObjectStoreObject], bool]] = None,
-    ) -> Generator[Tuple[ObjectStoreObject, ObjectStoreObject], None, None]:
+        prefilter_fn: Optional[Callable[[ObjectStoreObject], bool]] = None,  # TODO: change to StorageObject
+    ) -> Generator[TransferPair, None, None]:
         """Query source region and return list of objects to transfer.
 
         :param src_prefix: source bucket folder prefix
         :type src_prefix: string
         :param dst_prefix: destination bucket folder prefix
         :type dst_prefix: string
         :param recursive: if true, will copy objects at folder prefix recursively
         :type recursive: bool
         :param prefilter_fn: filters out objects whose prefixes do not match the filter function (default: None)
         :type prefilter_fn: Callable[[ObjectStoreObject], bool]
         """
+        if not isinstance(self.src_iface, ObjectStoreInterface) or not all(
+            [isinstance(dst_iface, ObjectStoreInterface) for dst_iface in self.dst_ifaces]
+        ):
+            raise NotImplementedError("TransferPair only supports object store interfaces")
+
         if not self.src_iface.bucket_exists():
             raise exceptions.MissingBucketException(f"Source bucket {self.src_iface.path()} does not exist or is not readable.")
-        if not self.dst_iface.bucket_exists():
-            raise exceptions.MissingBucketException(f"Destination bucket {self.dst_iface.path()} does not exist or is not readable.")
+        for dst_iface in self.dst_ifaces:
+            if not dst_iface.bucket_exists():
+                raise exceptions.MissingBucketException(f"Destination bucket {dst_iface.path()} does not exist or is not readable.")
 
         # query all source region objects
         logger.fs.debug(f"Querying objects in {self.src_iface.path()}")
         n_objs = 0
         for obj in self.src_iface.list_objects(src_prefix):
             if prefilter_fn is None or prefilter_fn(obj):
-                try:
-                    dest_key = self.map_object_key_prefix(src_prefix, obj.key, dst_prefix, recursive=recursive)
-                except exceptions.MissingObjectException as e:
-                    logger.fs.exception(e)
-                    raise e from None
-
-                # make destination object
-                dest_provider, dest_region = self.dst_iface.region_tag().split(":")
-                if dest_provider == "aws":
-                    dest_obj = S3Object(dest_provider, self.dst_iface.bucket(), dest_key)
-                elif dest_provider == "azure":
-                    dest_obj = AzureBlobObject(dest_provider, self.dst_iface.bucket(), dest_key)
-                elif dest_provider == "gcp":
-                    dest_obj = GCSObject(dest_provider, self.dst_iface.bucket(), dest_key)
-                else:
-                    raise ValueError(f"Invalid dest_region {dest_region}, unknown provider")
+                # collect list of destination objects
+                dest_objs = {}
+                dest_keys = []
+                for i in range(len(self.dst_ifaces)):
+                    dst_iface = self.dst_ifaces[i]
+                    dst_prefix = dst_prefixes[i]
+                    dest_provider, dest_region = dst_iface.region_tag().split(":")
+                    try:
+                        dest_key = self.map_object_key_prefix(src_prefix, obj.key, dst_prefix, recursive=recursive)
+                        assert (
+                            dest_key[: len(dst_prefix)] == dst_prefix
+                        ), f"Destination key {dest_key} does not start with destination prefix {dst_prefix}"
+                        dest_keys.append(dest_key[len(dst_prefix) :])
+                    except exceptions.MissingObjectException as e:
+                        logger.fs.exception(e)
+                        raise e from None
+
+                    if dest_provider == "aws":
+                        dest_obj = S3Object(provider=dest_provider, bucket=dst_iface.bucket(), key=dest_key)
+                    elif dest_provider == "azure":
+                        dest_obj = AzureBlobObject(provider=dest_provider, bucket=dst_iface.bucket(), key=dest_key)
+                    elif dest_provider == "gcp":
+                        dest_obj = GCSObject(provider=dest_provider, bucket=dst_iface.bucket(), key=dest_key)
+                    elif dest_provider == "cloudflare":
+                        dest_obj = R2Object(provider=dest_provider, bucket=dst_iface.bucket(), key=dest_key)
+                    else:
+                        raise ValueError(f"Invalid dest_region {dest_region}, unknown provider")
+                    dest_objs[dst_iface.region_tag()] = dest_obj
+
+                # assert that all destinations share the same post-fix key
+                assert len(list(set(dest_keys))) == 1, f"Destination keys {dest_keys} do not match"
                 n_objs += 1
-                yield obj, dest_obj
+                yield TransferPair(src_obj=obj, dst_objs=dest_objs, dst_key=dest_keys[0])
 
         if n_objs == 0:
             logger.error("Specified object does not exist.\n")
             raise exceptions.MissingObjectException(f"No objects were found in the specified prefix")
 
-    def chunk(
-        self, transfer_pair_generator: Generator[Tuple[ObjectStoreObject, ObjectStoreObject], None, None]
-    ) -> Generator[Chunk, None, None]:
+    def chunk(self, transfer_pair_generator: Generator[TransferPair, None, None]) -> Generator[GatewayMessage, None, None]:
         """Break transfer list into chunks.
 
         :param transfer_pair_generator: generator of pairs of objects to transfer
         :type transfer_pair_generator: Generator
         """
-        multipart_send_queue: Queue[Tuple[ObjectStoreObject, ObjectStoreObject]] = Queue()
-        multipart_chunk_queue: Queue[Chunk] = Queue()
+        multipart_send_queue: Queue[TransferPair] = Queue()
+        multipart_chunk_queue: Queue[GatewayMessage] = Queue()
         multipart_exit_event = threading.Event()
         multipart_chunk_threads = []
 
+        # TODO: remove after azure multipart implemented
+        azure_dest = any([dst_iface.provider == "azure" for dst_iface in self.dst_ifaces])
+
         # start chunking threads
-        if self.transfer_config.multipart_enabled:
+        if not azure_dest and self.transfer_config.multipart_enabled:
             for _ in range(self.concurrent_multipart_chunk_threads):
                 t = threading.Thread(
                     target=self._run_multipart_chunk_thread,
                     args=(multipart_exit_event, multipart_send_queue, multipart_chunk_queue),
                     daemon=False,
                 )
                 t.start()
                 multipart_chunk_threads.append(t)
 
         # begin chunking loop
-        for src_obj, dst_obj in transfer_pair_generator:
-            if self.transfer_config.multipart_enabled and src_obj.size > self.transfer_config.multipart_threshold_mb * MB:
-                multipart_send_queue.put((src_obj, dst_obj))
+        for transfer_pair in transfer_pair_generator:
+            # print("transfer_pair", transfer_pair.src_obj.key, transfer_pair.dst_objs)
+            src_obj = transfer_pair.src_obj
+            if (
+                not azure_dest
+                and self.transfer_config.multipart_enabled
+                and src_obj.size > self.transfer_config.multipart_threshold_mb * MB
+            ):
+                multipart_send_queue.put(transfer_pair)
             else:
-                yield Chunk(
-                    src_key=src_obj.key,
-                    dest_key=dst_obj.key,
-                    chunk_id=uuid.uuid4().hex,
-                    chunk_length_bytes=src_obj.size,
+                if transfer_pair.src_obj.size == 0:
+                    logger.fs.debug(f"Skipping empty object {src_obj.key}")
+                    continue
+                yield GatewayMessage(
+                    chunk=Chunk(
+                        src_key=src_obj.key,
+                        dest_key=transfer_pair.dst_key,  # TODO: get rid of dest_key, and have write object have info on prefix  (or have a map here)
+                        chunk_id=uuid.uuid4().hex,
+                        chunk_length_bytes=transfer_pair.src_obj.size,
+                        partition_id=str(0),  # TODO: fix this to distribute across multiple partitions
+                    )
                 )
 
             if self.transfer_config.multipart_enabled:
                 # drain multipart chunk queue and yield with updated chunk IDs
                 while not multipart_chunk_queue.empty():
                     yield multipart_chunk_queue.get()
 
         if self.transfer_config.multipart_enabled:
+            # wait for processing multipart requests to finish
+            logger.fs.debug("Waiting for multipart threads to finish")
+            # while not multipart_send_queue.empty():
+            # TODO: may be an issue waiting for this in case of force-quit
+            while not multipart_send_queue.empty():
+                logger.fs.debug(f"Remaining in multipart queue: sent {multipart_send_queue.qsize()}")
+                time.sleep(0.1)
             # send sentinel to all threads
             multipart_exit_event.set()
             for thread in multipart_chunk_threads:
                 thread.join()
 
             # drain multipart chunk queue and yield with updated chunk IDs
             while not multipart_chunk_queue.empty():
@@ -344,77 +447,105 @@
 @dataclass
 class TransferJob(ABC):
     """
     transfer job with transfer configurations
 
     :param src_path: source full path
     :type src_path: str
-    :param dst_path: destination full path
-    :type dst_path: str
+    :param dst_paths: destination full path
+    :type dst_paths: str
     :param recursive: if true, will transfer objects at folder prefix recursively (default: False)
     :type recursive: bool
     :param requester_pays: if set, will support requester pays buckets. (default: False)
     :type requester_pays: bool
     :param uuid: the uuid of one single transfer job
     :type uuid: str
     """
 
-    src_path: str
-    dst_path: str
-    recursive: bool = False
-    requester_pays: bool = False
-    uuid: str = field(init=False, default_factory=lambda: str(uuid.uuid4()))
+    # @abstractmethod
+    def __init__(
+        self,
+        src_path: str,
+        dst_paths: List[str] or str,
+        recursive: bool = False,
+        requester_pays: bool = False,
+        job_id: Optional[str] = None,
+    ):
+        self.src_path = src_path
+        self.dst_paths = dst_paths
+        self.recursive = recursive
+        self.requester_pays = requester_pays
+        if job_id is None:
+            self.uuid = str(uuid.uuid4())
+        else:
+            self.uuid = job_id
+
+    @property
+    def transfer_type(self) -> str:
+        if isinstance(self.dst_paths, str):
+            return "unicast"
+        else:
+            return "multicast"
 
     @property
     def src_prefix(self) -> Optional[str]:
         """Return the source prefix"""
         if not hasattr(self, "_src_prefix"):
             self._src_prefix = parse_path(self.src_path)[2]
         return self._src_prefix
 
     @property
-    def src_iface(self) -> ObjectStoreInterface:
+    def src_iface(self) -> StorageInterface:
         """Return the source object store interface"""
         if not hasattr(self, "_src_iface"):
             provider_src, bucket_src, _ = parse_path(self.src_path)
             self._src_iface = ObjectStoreInterface.create(f"{provider_src}:infer", bucket_src)
             if self.requester_pays:
                 self._src_iface.set_requester_bool(True)
         return self._src_iface
 
     @property
-    def dst_prefix(self) -> Optional[str]:
+    def dst_prefixes(self) -> List[str]:
         """Return the destination prefix"""
         if not hasattr(self, "_dst_prefix"):
-            self._dst_prefix = parse_path(self.dst_path)[2]
+            if self.transfer_type == "unicast":
+                self._dst_prefix = [str(parse_path(self.dst_paths[0])[2])]
+            else:
+                self._dst_prefix = [str(parse_path(path)[2]) for path in self.dst_paths]
         return self._dst_prefix
 
     @property
-    def dst_iface(self) -> ObjectStoreInterface:
+    def dst_ifaces(self) -> List[StorageInterface]:
         """Return the destination object store interface"""
         if not hasattr(self, "_dst_iface"):
-            provider_dst, bucket_dst, _ = parse_path(self.dst_path)
-            self._dst_iface = ObjectStoreInterface.create(f"{provider_dst}:infer", bucket_dst)
-        return self._dst_iface
+            if self.transfer_type == "unicast":
+                provider_dst, bucket_dst, _ = parse_path(self.dst_paths[0])
+                self._dst_ifaces = [StorageInterface.create(f"{provider_dst}:infer", bucket_dst)]
+            else:
+                self._dst_ifaces = []
+                for path in self.dst_paths:
+                    provider_dst, bucket_dst, _ = parse_path(path)
+                    self._dst_ifaces.append(StorageInterface.create(f"{provider_dst}:infer", bucket_dst))
+        return self._dst_ifaces
 
-    def dispatch(self, dataplane: "Dataplane", **kwargs) -> Generator[ChunkRequest, None, None]:
+    def dispatch(self, dataplane: "Dataplane", **kwargs) -> Generator[Chunk, None, None]:
         """Dispatch transfer job to specified gateways."""
         raise NotImplementedError("Dispatch not implemented")
 
     def finalize(self):
         """Complete the multipart upload requests"""
         raise NotImplementedError("Finalize not implemented")
 
     def verify(self):
         """Verifies the transfer completed, otherwise raises TransferFailedException."""
         raise NotImplementedError("Verify not implemented")
 
-    def estimate_cost(self):
-        # TODO
-        raise NotImplementedError
+    def size_gb(self):
+        """Return the size of the transfer in GB"""
+        raise NotImplementedError("Size not implemented")
 
     @classmethod
     def _pre_filter_fn(cls, obj: ObjectStoreObject) -> bool:
         """Optionally filter source objects before they are transferred.
 
         :meta private:
         :param obj: source object to be transferred
@@ -429,166 +560,277 @@
 
     :param transfer_list: transfer list for later verification
     :type transfer_list: list
     :param multipart_transfer_list: multipart transfer list for later verification
     :type multipart_transfer_list: list
     """
 
-    transfer_list: list = field(default_factory=list)
-    multipart_transfer_list: list = field(default_factory=list)
+    def __init__(
+        self,
+        src_path: str,
+        dst_paths: List[str] or str,
+        recursive: bool = False,
+        requester_pays: bool = False,
+        job_id: Optional[str] = None,
+    ):
+        super().__init__(src_path, dst_paths, recursive, requester_pays, job_id)
+        self.transfer_list = []
+        self.multipart_transfer_list = []
 
     @property
     def http_pool(self):
         """http connection pool"""
         if not hasattr(self, "_http_pool"):
-            self._http_pool = urllib3.PoolManager(retries=urllib3.Retry(total=3))
+            timeout = urllib3.util.Timeout(connect=10.0, read=None)  # no read timeout
+            self._http_pool = urllib3.PoolManager(retries=urllib3.Retry(total=3), timeout=timeout)
         return self._http_pool
 
-    def estimate_cost(self):
-        raise NotImplementedError()
-
-    def gen_transfer_pairs(self, chunker: Optional[Chunker] = None) -> Generator[Tuple[ObjectStoreObject, ObjectStoreObject], None, None]:
+    def gen_transfer_pairs(
+        self,
+        chunker: Optional[Chunker] = None,
+        transfer_config: Optional[TransferConfig] = field(init=False, default_factory=lambda: TransferConfig()),
+    ) -> Generator[TransferPair, None, None]:
         """Generate transfer pairs for the transfer job.
 
         :param chunker: chunker that makes the chunk requests
         :type chunker: Chunker
         """
         if chunker is None:  # used for external access to transfer pair list
-            chunker = Chunker(self.src_iface, self.dst_iface, TransferConfig())
-        yield from chunker.transfer_pair_generator(self.src_prefix, self.dst_prefix, self.recursive, self._pre_filter_fn)
+            chunker = Chunker(self.src_iface, self.dst_ifaces, transfer_config)  # TODO: should read in existing transfer config
+        yield from chunker.transfer_pair_generator(self.src_prefix, self.dst_prefixes, self.recursive, self._pre_filter_fn)
 
     def dispatch(
         self,
         dataplane: "Dataplane",
-        transfer_config: TransferConfig,
         dispatch_batch_size: int = 100,  # 6.4 GB worth of chunks
-    ) -> Generator[ChunkRequest, None, None]:
+        transfer_config: Optional[TransferConfig] = field(init=False, default_factory=lambda: TransferConfig()),
+    ) -> Generator[Chunk, None, None]:
         """Dispatch transfer job to specified gateways.
 
         :param dataplane: dataplane that starts the transfer job
         :type dataplane: Dataplane
         :param transfer_config: the configuration during the transfer
         :type transfer_config: TransferConfig
         :param dispatch_batch_size: maximum size of the buffer to temporarily store the generators (default: 1000)
         :type dispatch_batch_size: int
         """
-        chunker = Chunker(self.src_iface, self.dst_iface, transfer_config)
-        transfer_pair_generator = self.gen_transfer_pairs(chunker)
+        chunker = Chunker(self.src_iface, self.dst_ifaces, transfer_config)
+        transfer_pair_generator = self.gen_transfer_pairs(chunker)  # returns TransferPair objects
         gen_transfer_list = chunker.tail_generator(transfer_pair_generator, self.transfer_list)
         chunks = chunker.chunk(gen_transfer_list)
-        chunk_requests = chunker.to_chunk_requests(chunks)
-
         batches = chunker.batch_generator(
-            chunker.prefetch_generator(chunk_requests, buffer_size=dispatch_batch_size * 32), batch_size=dispatch_batch_size
+            chunker.prefetch_generator(chunks, buffer_size=dispatch_batch_size * 32), batch_size=dispatch_batch_size
         )
 
         # dispatch chunk requests
         src_gateways = dataplane.source_gateways()
-        bytes_dispatched = [0] * len(src_gateways)
+        queue_size = [0] * len(src_gateways)
         n_multiparts = 0
         start = time.time()
+
         for batch in batches:
-            end = time.time()
-            logger.fs.debug(f"Queried {len(batch)} chunks in {end - start:.2f} seconds")
-            start = time.time()
-            min_idx = bytes_dispatched.index(min(bytes_dispatched))
-            server = src_gateways[min_idx]
-            n_bytes = sum([cr.chunk.chunk_length_bytes for cr in batch])
-            bytes_dispatched[min_idx] += n_bytes
-            start = time.time()
-            reply = self.http_pool.request(
-                "POST",
-                f"{server.gateway_api_url}/api/v1/chunk_requests",
-                body=json.dumps([c.as_dict() for c in batch]).encode("utf-8"),
-                headers={"Content-Type": "application/json"},
-            )
-            end = time.time()
-            if reply.status != 200:
-                raise Exception(f"Failed to dispatch chunk requests {server.instance_name()}: {reply.data.decode('utf-8')}")
-            logger.fs.debug(
-                f"Dispatched {len(batch)} chunk requests to {server.instance_name()} ({n_bytes} bytes) in {end - start:.2f} seconds"
-            )
-            yield from batch
+            # send upload_id mappings to sink gateways
+            upload_id_batch = [cr for cr in batch if cr.upload_id_mapping is not None]
+            region_dst_gateways = dataplane.sink_gateways()
+            for region_tag, dst_gateways in region_dst_gateways.items():
+                for dst_gateway in dst_gateways:
+                    # collect upload id mappings
+                    mappings = {}
+                    for message in upload_id_batch:
+                        for region_tag, (key, id) in message.upload_id_mapping.items():
+                            if region_tag not in mappings:
+                                mappings[region_tag] = {}
+                            mappings[region_tag][key] = id
+
+                    # send mapping to gateway
+                    reply = self.http_pool.request(
+                        "POST",
+                        f"{dst_gateway.gateway_api_url}/api/v1/upload_id_maps",
+                        body=json.dumps(mappings).encode("utf-8"),
+                        headers={"Content-Type": "application/json"},
+                    )
+                    # TODO: assume that only destination nodes would write to the obj store
+                    if reply.status != 200:
+                        raise Exception(
+                            f"Failed to update upload ids to the dst gateway {dst_gateway.instance_name()}: {reply.data.decode('utf-8')}"
+                        )
+
+            # send chunk requests to source gateways
+            chunk_batch = [cr.chunk for cr in batch if cr.chunk is not None]
+            # TODO: allow multiple partition ids per chunk
+            for chunk in chunk_batch:  # assign job UUID as partition ID
+                chunk.partition_id = self.uuid
+            min_idx = queue_size.index(min(queue_size))
+            n_added = 0
+            while n_added < len(chunk_batch):
+                # TODO: should update every source instance queue size
+                server = src_gateways[min_idx]
+                assert Chunk.from_dict(chunk_batch[0].as_dict()) == chunk_batch[0], f"Invalid chunk request: {chunk_batch[0].as_dict}"
+
+                # TODO: make async
+                st = time.time()
+                reply = self.http_pool.request(
+                    "POST",
+                    f"{server.gateway_api_url}/api/v1/chunk_requests",
+                    body=json.dumps([chunk.as_dict() for chunk in chunk_batch[n_added:]]).encode("utf-8"),
+                    headers={"Content-Type": "application/json"},
+                )
+                if reply.status != 200:
+                    raise Exception(f"Failed to dispatch chunk requests {server.instance_name()}: {reply.data.decode('utf-8')}")
+                et = time.time()
+                reply_json = json.loads(reply.data.decode("utf-8"))
+                n_added += reply_json["n_added"]
+                logger.fs.debug(f"Added {n_added} chunks to server {server} in {et-st}: {reply_json}")
+                queue_size[min_idx] = reply_json["qsize"]  # update queue size
+                # dont try again with some gateway
+                min_idx = (min_idx + 1) % len(src_gateways)
+
+            yield from chunk_batch
 
             # copy new multipart transfers to the multipart transfer list
             updated_len = len(chunker.multipart_upload_requests)
             self.multipart_transfer_list.extend(chunker.multipart_upload_requests[n_multiparts:updated_len])
             n_multiparts = updated_len
 
     def finalize(self):
         """Complete the multipart upload requests"""
+        typer.secho(f"Finalizing multipart uploads...", fg="bright_black")
         groups = defaultdict(list)
         for req in self.multipart_transfer_list:
             if "region" not in req or "bucket" not in req:
                 raise Exception(f"Invalid multipart upload request: {req}")
             groups[(req["region"], req["bucket"])].append(req)
         for key, group in groups.items():
             region, bucket = key
             batch_len = max(1, len(group) // 128)
             batches = [group[i : i + batch_len] for i in range(0, len(group), batch_len)]
-            obj_store_interface = ObjectStoreInterface.create(region, bucket)
+            obj_store_interface = StorageInterface.create(region, bucket)
 
             def complete_fn(batch):
                 for req in batch:
-                    obj_store_interface.complete_multipart_upload(req["key"], req["upload_id"])
+                    logger.fs.debug(f"Finalize upload id {req['upload_id']} for key {req['key']}")
+                    retry_backoff(
+                        partial(obj_store_interface.complete_multipart_upload, req["key"], req["upload_id"], req["metadata"]),
+                        initial_backoff=0.5,
+                    )
 
-            do_parallel(complete_fn, batches, n=-1)
+            do_parallel(complete_fn, batches, n=8)
+
+        # TODO: Do NOT do this if we are pipelining multiple transfers - remove just what was completed
+        self.multipart_transfer_list = []
 
     def verify(self):
         """Verify the integrity of the transfered destination objects"""
-        dst_keys = {dst_o.key: src_o for src_o, dst_o in self.transfer_list}
-        for obj in self.dst_iface.list_objects(self.dst_prefix):
-            # check metadata (src.size == dst.size) && (src.modified <= dst.modified)
-            src_obj = dst_keys.get(obj.key)
-            if src_obj and src_obj.size == obj.size and src_obj.last_modified <= obj.last_modified:
-                del dst_keys[obj.key]
-        if dst_keys:
-            failed_keys = [obj.key for obj in dst_keys.values()]
-            raise exceptions.TransferFailedException(f"{len(dst_keys)} objects failed verification {failed_keys}")
+
+        def verify_region(i):
+            dst_iface = self.dst_ifaces[i]
+            dst_prefix = self.dst_prefixes[i]
+
+            # gather destination key mapping for this region
+            dst_keys = {pair.dst_objs[dst_iface.region_tag()].key: pair.src_obj for pair in self.transfer_list}
+
+            # list and check destination prefix
+            for obj in dst_iface.list_objects(dst_prefix):
+                # check metadata (src.size == dst.size) && (src.modified <= dst.modified)
+                src_obj = dst_keys.get(obj.key)
+                if src_obj and src_obj.size == obj.size and src_obj.last_modified <= obj.last_modified:
+                    del dst_keys[obj.key]
+
+            if dst_keys:
+                # failed_keys = [obj.key for obj in dst_keys.values()]
+                failed_keys = list(dst_keys.keys())
+                if failed_keys == [""]:
+                    return  # ignore empty key
+                raise exceptions.TransferFailedException(
+                    f"Destination {dst_iface.region_tag()} bucket {dst_iface.bucket()}: {len(dst_keys)} objects failed verification {failed_keys}"
+                )
+
+        n = 1  # number threads
+        assert n == 1, "Only use one thread for verifying objects: n>1 causes concurrency error"
+        do_parallel(
+            verify_region,
+            range(len(self.dst_ifaces)),
+            spinner=True,
+            spinner_persist=False,
+            desc="Verifying objects in destination buckets",
+            n=n,
+        )
+
+    def size_gb(self):
+        """Return the size of the transfer in GB"""
+        total_size = 0
+        for pair in self.gen_transfer_pairs():
+            total_size += pair.src_obj.size
+        return total_size / 1e9
 
 
 @dataclass
 class SyncJob(CopyJob):
     """sync job that copies the source objects that does not exist in the destination bucket to the destination"""
 
-    def estimate_cost(self):
-        raise NotImplementedError()
+    def __init__(self, src_path: str, dst_paths: List[str] or str, requester_pays: bool = False, job_id: Optional[str] = None):
+        super().__init__(src_path, dst_paths, True, requester_pays, job_id)
+        self.transfer_list = []
+        self.multipart_transfer_list = []
+
+        assert isinstance(self.src_iface, ObjectStoreInterface), "Source must be an object store interface"
+        assert not any(
+            [not isinstance(iface, ObjectStoreInterface) for iface in self.dst_ifaces]
+        ), "Destination must be a object store interface"
 
-    def gen_transfer_pairs(self, chunker: Optional[Chunker] = None) -> Generator[Tuple[ObjectStoreObject, ObjectStoreObject], None, None]:
+    def gen_transfer_pairs(
+        self,
+        chunker: Optional[Chunker] = None,
+        transfer_config: Optional[TransferConfig] = field(init=False, default_factory=lambda: TransferConfig()),
+    ) -> Generator[TransferPair, None, None]:
         """Generate transfer pairs for the transfer job.
 
         :param chunker: chunker that makes the chunk requests
         :type chunker: Chunker
         """
         if chunker is None:  # used for external access to transfer pair list
-            chunker = Chunker(self.src_iface, self.dst_iface, TransferConfig())
-        transfer_pair_gen = chunker.transfer_pair_generator(self.src_prefix, self.dst_prefix, self.recursive, self._pre_filter_fn)
+            chunker = Chunker(self.src_iface, self.dst_ifaces, transfer_config)
+        transfer_pair_gen = chunker.transfer_pair_generator(self.src_prefix, self.dst_prefixes, self.recursive, self._pre_filter_fn)
+
+        # only single destination supported
+        assert len(self.dst_ifaces) == 1, "Only single destination supported for sync job"
+
         # enrich destination objects with metadata
-        for src_obj, dest_obj in self._enrich_dest_objs(transfer_pair_gen, self.dst_prefix):
+        for src_obj, dest_obj in self._enrich_dest_objs(transfer_pair_gen, self.dst_prefixes):
             if self._post_filter_fn(src_obj, dest_obj):
-                yield src_obj, dest_obj
+                yield TransferPair(
+                    src_obj=src_obj,
+                    dst_objs={self.dst_ifaces[0].region_tag(): dest_obj},
+                    dst_key=dest_obj.key.replace(self.dst_prefixes[0], ""),
+                )
 
     def _enrich_dest_objs(
-        self, transfer_pairs: Generator[Tuple[ObjectStoreObject, ObjectStoreObject], None, None], dest_prefix: str
+        self, transfer_pairs: Generator[TransferPair, None, None], dest_prefixes: List[str]
     ) -> Generator[Tuple[ObjectStoreObject, ObjectStoreObject], None, None]:
         """
         For skyplane sync, we enrich dest obj metadata with our existing dest obj metadata from the dest bucket following a query.
 
         :meta private:
         :param transfer_pairs: generator of transfer pairs
         :type transfer_pairs: Generator
         """
-        logger.fs.debug(f"Querying objects in {self.dst_iface.bucket()}")
-        if not hasattr(self, "_found_dest_objs"):
-            self._found_dest_objs = {obj.key: obj for obj in self.dst_iface.list_objects(dest_prefix)}
-        for src_obj, dest_obj in transfer_pairs:
-            if dest_obj.key in self._found_dest_objs:
-                dest_obj.size = self._found_dest_objs[dest_obj.key].size
-                dest_obj.last_modified = self._found_dest_objs[dest_obj.key].last_modified
-            yield src_obj, dest_obj
+        for i in range(len(self.dst_ifaces)):
+            dst_iface = self.dst_ifaces[i]
+            dest_prefix = dest_prefixes[i]
+            logger.fs.debug(f"Querying objects in {dst_iface.bucket()}")
+            if not hasattr(self, "_found_dest_objs"):
+                self._found_dest_objs = {obj.key: obj for obj in dst_iface.list_objects(dest_prefix)}
+            for pair in transfer_pairs:
+                src_obj = pair.src_obj
+                dest_obj = list(pair.dst_objs.values())[0]
+                assert len(list(pair.dst_objs.keys())) == 1, f"Multiple destinations are not support for sync: {pair.dst_objs}"
+                if dest_obj.key in self._found_dest_objs:
+                    dest_obj.size = self._found_dest_objs[dest_obj.key].size
+                    dest_obj.last_modified = self._found_dest_objs[dest_obj.key].last_modified
+                yield src_obj, dest_obj
 
     @classmethod
     def _post_filter_fn(cls, src_obj: ObjectStoreObject, dest_obj: ObjectStoreObject) -> bool:
         """Optionally filter destination objects after they are transferred.
 
         :param src_obj: source object to be transferred
         :type src_obj: ObjectStoreObject
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/api/usage.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/api/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import configparser
 from dataclasses import asdict, dataclass
 from enum import Enum, auto
 from pathlib import Path
 
 import requests
 from rich import print as rprint
-from typing import Optional, Dict
+from typing import Optional, Dict, List
 
 import skyplane
 from skyplane.utils.definitions import tmp_log_dir
 from skyplane.config import _map_type
 from skyplane.config_paths import config_path, cloud_config, host_uuid_path
 from skyplane.utils import logger, imports
 
@@ -89,15 +89,15 @@
     #: The client id from SkyplaneConfig.
     client_id: Optional[str]
     #: A random id of the transfer session with time.
     session_id: str
     #: The source region of the transfer session.
     source_region: str
     #: The destination region of the transfer session.
-    destination_region: str
+    destination_region: str  # TODO: make into dest_regions
     #: The source cloud provider of the transfer session.
     source_cloud_provider: str
     #: The destination cloud provider of the transfer session.
     destination_cloud_provider: str
     #: The operating system in use.
     os: str
     #: When the transfer is started.
@@ -132,15 +132,15 @@
     @classmethod
     def log_exception(
         cls,
         location: str,
         exception: Exception,
         args: Optional[Dict] = None,
         src_region_tag: Optional[str] = None,
-        dest_region_tag: Optional[str] = None,
+        dest_region_tag: Optional[str] = None,  # TODO: fix this for mult-dest
         session_start_timestamp_ms: Optional[int] = None,
     ):
         if cls.enabled():
             client = cls()
             error_dict = {"loc": location, "message": str(exception)[:150]}
             stats = client.make_error(
                 error_dict=error_dict,
@@ -154,24 +154,24 @@
 
     @classmethod
     def log_transfer(
         cls,
         transfer_stats: Optional[Dict],
         args: Optional[Dict] = None,
         src_region_tag: Optional[str] = None,
-        dest_region_tag: Optional[str] = None,
+        dest_region_tags: Optional[str] = None,
         session_start_timestamp_ms: Optional[int] = None,
     ):
         if cls.enabled():
             client = cls()
             stats = client.make_stat(
                 arguments_dict=args,
                 transfer_stats=transfer_stats,
                 src_region_tag=src_region_tag,
-                dest_region_tag=dest_region_tag,
+                dest_region_tags=dest_region_tags,
                 session_start_timestamp_ms=session_start_timestamp_ms,
             )
             destination = client.write_usage_data(stats)
             client.report_usage_data("usage", stats, destination)
 
     @classmethod
     def usage_stats_status(cls) -> UsageStatsStatus:
@@ -246,25 +246,26 @@
             rprint(USAGE_STATS_REENABLED_MESSAGE)
 
     def make_stat(
         self,
         arguments_dict: Optional[Dict] = None,
         transfer_stats: Optional[Dict] = None,
         src_region_tag: Optional[str] = None,
-        dest_region_tag: Optional[str] = None,
+        dest_region_tags: Optional[str] = None,
         session_start_timestamp_ms: Optional[int] = None,
     ):
         if src_region_tag is None:
             src_provider, src_region = None, None
         else:
             src_provider, src_region = src_region_tag.split(":")
-        if dest_region_tag is None:
+        if dest_region_tags is None:
             dest_provider, dest_region = None, None
         else:
-            dest_provider, dest_region = dest_region_tag.split(":")
+            # TODO: have usage stats view for multiple destinations
+            dest_provider, dest_region = dest_region_tags[0].split(":")
 
         return UsageStatsToReport(
             skyplane_version=skyplane.__version__,
             python_version=".".join(map(str, sys.version_info[:3])),
             schema_version=SCHEMA_VERSION,
             client_id=self.client_id,
             session_id=self.session_id,
@@ -286,29 +287,30 @@
         dest_region_tag: Optional[str] = None,
         session_start_timestamp_ms: Optional[int] = None,
     ):
         if src_region_tag is None:
             src_provider, src_region = None, None
         else:
             src_provider, src_region = src_region_tag.split(":")
+
         if dest_region_tag is None:
             dest_provider, dest_region = None, None
         else:
             dest_provider, dest_region = dest_region_tag.split(":")
 
         return UsageStatsToReport(
             skyplane_version=skyplane.__version__,
             python_version=".".join(map(str, sys.version_info[:3])),
             schema_version=SCHEMA_VERSION,
             client_id=self.client_id,
             session_id=self.session_id,
             source_region=src_region,
-            destination_region=dest_region,
+            destination_region=dest_region,  # TODO: fix this
             source_cloud_provider=src_provider,
-            destination_cloud_provider=dest_provider,
+            destination_cloud_provider=dest_provider,  # TODO: FIX THIS
             os=sys.platform,
             session_start_timestamp_ms=session_start_timestamp_ms if session_start_timestamp_ms else int(time.time() * 1000),
             arguments_dict=arguments_dict,
             error_dict=error_dict,
         )
 
     def write_usage_data(self, data: UsageStatsToReport, dir_path: Optional[Path] = None):
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/cert.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/cert.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_daemon.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_daemon.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,64 @@
 import argparse
+from multiprocessing import Manager
+from pprint import pprint
 import atexit
 import json
 import os
 import signal
 import sys
-import time
-from collections import defaultdict
 from multiprocessing import Event, Queue
 from os import PathLike
 from pathlib import Path
-from pprint import pprint
-from typing import Dict
+from typing import Dict, List, Optional
 
-from skyplane.broadcast.gateway.chunk_store import ChunkStore
-from skyplane.broadcast.gateway.gateway_daemon_api import GatewayDaemonAPI
-from skyplane.broadcast.gateway.gateway_queue import GatewayANDQueue, GatewayORQueue
-from skyplane.broadcast.gateway.operators.gateway_operator import (
-    GatewayWaitReciever,
-    GatewayObjStoreReadOperator,
-    GatewayRandomDataGen,
+from skyplane.utils import logger
+
+from skyplane.gateway.gateway_queue import GatewayQueue, GatewayANDQueue
+from skyplane.gateway.chunk_store import ChunkStore
+from skyplane.gateway.gateway_daemon_api import GatewayDaemonAPI
+from skyplane.gateway.operators.gateway_operator import (
     GatewaySender,
-    GatewayObjStoreWriteOperator,
+    GatewayRandomDataGen,
     GatewayWriteLocal,
+    GatewayObjStoreReadOperator,
+    GatewayObjStoreWriteOperator,
+    GatewayWaitReciever,
 )
-from skyplane.broadcast.gateway.operators.gateway_receiver import GatewayReceiver
+from skyplane.gateway.operators.gateway_receiver import GatewayReceiver
 from skyplane.utils import logger
-
-# TODO: add default partition ID to main
-# create gateway broadcast
+from collections import defaultdict
 
 
+# TODO: add default partition ID to main
+# create gateway br
 class GatewayDaemon:
     def __init__(
         self,
         region: str,
         chunk_dir: PathLike,
         max_incoming_ports=64,
         use_tls=True,
         use_e2ee=False,
     ):
         # read gateway program
         gateway_program_path = Path(os.environ["GATEWAY_PROGRAM_FILE"]).expanduser()
         gateway_program = json.load(open(gateway_program_path, "r"))
 
-        print(gateway_program)
+        self.upload_id_map = Manager().dict()
+
+        pprint(gateway_program)
+
+        # read gateway info
+        gateway_info_path = Path(os.environ["GATEWAY_INFO_FILE"]).expanduser()
+        self.gateway_info = json.load(open(gateway_info_path, "r"))
+
+        print("starting gateway daemon", gateway_program_path)
+        pprint(gateway_program)
+        assert len(gateway_program) > 0, f"Cannot have empty gateway program {gateway_program}"
 
         self.use_tls = use_tls
 
         # todo max_incoming_ports should be configurable rather than static
         self.region = region
         self.max_incoming_ports = max_incoming_ports
 
@@ -61,169 +72,241 @@
             with open(e2ee_key_path, "rb") as f:
                 self.e2ee_key_bytes = f.read()
         else:
             self.e2ee_key_bytes = None
 
         # create gateway operators
         self.terminal_operators = defaultdict(list)  # track terminal operators per partition
-        self.operators = self.create_gateway_operators(gateway_program["_plan"])
+        self.num_required_terminal = {}
+        self.operators = self.create_gateway_operators(gateway_program)
 
         # single gateway reciever
-        print("create gateway reciever")
         self.gateway_receiver = GatewayReceiver(
             "reciever",
             region=region,
             chunk_store=self.chunk_store,
             error_event=self.error_event,
             error_queue=self.error_queue,
             max_pending_chunks=max_incoming_ports,
             use_tls=self.use_tls,
             use_compression=False,  # use_compression,
             e2ee_key_bytes=self.e2ee_key_bytes,
         )
 
         # API server
         self.api_server = GatewayDaemonAPI(
-            self.chunk_store, self.gateway_receiver, self.error_event, self.error_queue, self.terminal_operators
+            self.chunk_store,
+            self.gateway_receiver,
+            self.error_event,
+            self.error_queue,
+            terminal_operators=self.terminal_operators,
+            num_required_terminal=self.num_required_terminal,
+            upload_id_map=self.upload_id_map,
         )
         self.api_server.start()
         atexit.register(self.api_server.shutdown)
         logger.info(f"[gateway_daemon] API started at {self.api_server.url}")
 
+    def print_operator_graph(self):
+        def print_operator_graph_helper(partition, queue: GatewayQueue, prefix: str):
+            if queue is None:
+                return
+            print(f"{prefix} {partition}: Input queue:", queue, "handles:", queue.get_handles())
+            for handle in queue.get_handles():
+                print(f"{prefix} {partition}: Operator {handle}")
+                # TODO: causes error sometimes for mux_or
+                next_queue = self.operators[handle].output_queue
+                print_operator_graph_helper(partition, next_queue, prefix + "--")
+
+        for partition, queue in self.chunk_store.chunk_requests.items():
+            print(f"Partition {partition}, {queue}")
+            print_operator_graph_helper(partition, queue, "")
+
     def create_gateway_operators(self, gateway_program: Dict):
         """Create a gateway plan from a gateway program"""
 
         operators = {}
 
         def create_output_queue(operator: Dict):
             # create output data queue
-            print("DETERMINING OUTPUT QUEUE", operator["children"])
             if len(operator["children"]) == 0:
                 return None
+            print("get output queue", operator["op_type"], operator["children"][0]["op_type"])
             if operator["children"][0]["op_type"] == "mux_and":
                 return GatewayANDQueue()
-            return GatewayORQueue()
+            return GatewayQueue()
 
         def get_child_operators(operator):
             if len(operator["children"]) == 0:
                 return []
             if operator["children"][0]["op_type"] == "mux_and" or operator["children"][0]["op_type"] == "mux_or":
                 return operator["children"][0]["children"]
             return operator["children"]
 
-        def create_gateway_operators_helper(input_queue, program: Dict, partition_id: str):
-            print("OPERATORS", operators)
+        def create_gateway_operators_helper(input_queue, program: List[Dict], partition_ids: List[str]):
+            total_p = 0
             for op in program:
-                handle = op["handle"]
+                handle = op["op_type"] + "_" + op["handle"]
+                print(f"Input queue {input_queue}, adding handle {handle} (current handles {input_queue.get_handles()}")
                 input_queue.register_handle(handle)
-                print("INPUT QUEUE", input_queue, input_queue.get_handles())
+
+                # get child operators
+                child_operators = get_child_operators(op)
+
+                if op["op_type"] == "mux_or":
+                    # parent must have been mux_and
+                    assert isinstance(
+                        input_queue, GatewayANDQueue
+                    ), f"Parent must have been mux_and {handle}, instead was {input_queue} {gateway_program}"
+
+                    # recurse to children with single queue
+                    total_p += create_gateway_operators_helper(input_queue.get_handle_queue(handle), child_operators, partition_ids)
+                    continue
+
                 # create output data queue
                 output_queue = create_output_queue(op)
+                if isinstance(output_queue, GatewayANDQueue):
+                    # update number of operations that must be completed
+                    for partition in partition_ids:
+                        self.num_required_terminal[str(partition)] = self.num_required_terminal[str(partition)] - 1 + len(child_operators)
+
+                print(f"Input queue {input_queue} handle {handle}: created output queue {output_queue}")
+                print(f"Input queue {input_queue} handle {handle}: has children {child_operators}")
                 if output_queue is None:
                     # track what opeartors need to complete processing the chunk
-                    self.terminal_operators[partition_id].append(op["handle"])
-
-                # get child operators
-                child_operators = get_child_operators(op)
+                    for partition in partition_ids:
+                        self.terminal_operators[str(partition)].append(handle)
 
                 # create operators
                 if op["op_type"] == "receive":
                     # wait for chunks from reciever
                     operators[handle] = GatewayWaitReciever(
                         handle=handle,
                         region=self.region,
                         input_queue=input_queue,
                         output_queue=output_queue,
-                        n_processes=1,
+                        n_processes=1,  # dummy wait thread, not actual reciever
                         chunk_store=self.chunk_store,
                         error_event=self.error_event,
                         error_queue=self.error_queue,
                     )
+                    total_p += 1
                 elif op["op_type"] == "read_object_store":
                     operators[handle] = GatewayObjStoreReadOperator(
                         handle=handle,
                         region=self.region,
                         input_queue=input_queue,
                         output_queue=output_queue,
                         error_queue=self.error_queue,
                         error_event=self.error_event,
                         n_processes=op["num_connections"],
                         chunk_store=self.chunk_store,
                         bucket_name=op["bucket_name"],
                         bucket_region=op["bucket_region"],
                     )
+                    total_p += op["num_connections"]
                 elif op["op_type"] == "gen_data":
                     operators[handle] = GatewayRandomDataGen(
                         handle=handle,
                         region=self.region,
                         input_queue=input_queue,
                         output_queue=output_queue,
                         error_queue=self.error_queue,
                         error_event=self.error_event,
                         chunk_store=self.chunk_store,
                         size_mb=op["size_mb"],
                     )
                 elif op["op_type"] == "send":
+                    # TODO: handle private ips for GCP->GCP
+                    target_gateway_info = self.gateway_info[op["target_gateway_id"]]
+                    ip_addr = target_gateway_info["private_ip_address"] if op["private_ip"] else target_gateway_info["public_ip_address"]
+                    print("Gateway sender sending to ", ip_addr, "private", op["private_ip"])
                     operators[handle] = GatewaySender(
                         handle,
                         region=self.region,
-                        ip_addr=op["ip_address"],
+                        ip_addr=ip_addr,
                         input_queue=input_queue,
                         output_queue=output_queue,
                         error_event=self.error_event,
                         error_queue=self.error_queue,
                         chunk_store=self.chunk_store,
                         use_tls=self.use_tls,
                         use_compression=False,  # operator["compress"],
                         e2ee_key_bytes=self.e2ee_key_bytes,
                         n_processes=op["num_connections"],
                     )
+                    total_p += op["num_connections"]
                 elif op["op_type"] == "write_object_store":
                     operators[handle] = GatewayObjStoreWriteOperator(
                         handle=handle,
                         region=self.region,
                         input_queue=input_queue,
                         output_queue=output_queue,
                         error_queue=self.error_queue,
                         error_event=self.error_event,
                         n_processes=op["num_connections"],
                         chunk_store=self.chunk_store,
                         bucket_name=op["bucket_name"],
                         bucket_region=op["bucket_region"],
+                        upload_id_map=self.upload_id_map,
+                        prefix=op["key_prefix"],
                     )
+                    total_p += op["num_connections"]
                 elif op["op_type"] == "write_local":
                     operators[handle] = GatewayWriteLocal(
                         handle=handle,
                         region=self.region,
                         input_queue=input_queue,
                         output_queue=output_queue,
                         error_queue=self.error_queue,
                         error_event=self.error_event,
                         chunk_store=self.chunk_store,
                     )
+                    total_p += 1
                 else:
                     raise ValueError(f"Unsupported op_type {op['op_type']}")
                 # recursively create for child operators
-                create_gateway_operators_helper(output_queue, child_operators, partition_id)
+                total_p += create_gateway_operators_helper(output_queue, child_operators, partition_ids)
+            return total_p
 
-        print("GATEWAY PROGRAM")
         pprint(gateway_program)
 
         # create operator tree for each partition
-        for partition, program in gateway_program.items():
-            partition = str(partition)
+        total_p = 0
+        for program_group in gateway_program:
+            partitions = program_group["partitions"]
+            program = program_group["value"]
 
+            print("partitions", partitions)
             # create initial queue for partition
-            self.chunk_store.add_partition(partition)
-
-            create_gateway_operators_helper(
-                self.chunk_store.chunk_requests[partition],  # incoming chunk requests for partition
+            if program[0]["op_type"] == "mux_and":
+                queue = GatewayANDQueue()
+                print(f"First operator is mux_and: queue {queue}")
+                assert len(program) == 1, f"mux_and cannot have siblings"
+                program = program[0]["children"]
+                for partition in partitions:
+                    self.num_required_terminal[str(partition)] = len(program)
+            else:
+                queue = GatewayQueue()
+                print(f"First operator is ", program[0], "queue", queue)
+
+                for partition in partitions:
+                    self.num_required_terminal[str(partition)] = 1
+
+            # link all partitions to same queue reference
+            for partition in partitions:
+                self.chunk_store.add_partition(str(partition), queue)
+
+            # create DAG for this partition group
+            total_p += create_gateway_operators_helper(
+                self.chunk_store.chunk_requests[str(partition)],  # incoming chunk requests for partition
                 program,  # single partition program
-                partition,
+                partitions,
             )
+        # print("TOTAL NUMBER OF PROCESSES", total_p)
         return operators
 
     def run(self):
         exit_flag = Event()
 
         def exit_handler(signum, frame):
             logger.warning("[gateway_daemon] Received signal {}. Exiting...".format(signum))
@@ -237,52 +320,16 @@
             operator.start_workers()
 
         signal.signal(signal.SIGINT, exit_handler)
         signal.signal(signal.SIGTERM, exit_handler)
 
         logger.info("[gateway_daemon] Starting daemon loop")
         try:
-            print(self.operators)
             while not exit_flag.is_set() and not self.error_event.is_set():
-                print("pull queue...")
                 self.api_server.pull_chunk_status_queue()
-                # pull from chunk requests queue
-                # print("running gateway daemon... nothing to do")
-                # while True:
-                #    try:
-                #        chunk_req = self.chunk_store.chunk_requests.get_nowait()
-                #    except Empty:
-                #        break
-
-                #    print("registered chunk", chunk_req.chunk.chunk_id, "partition", chunk_req.chunk.partition_id)
-                #    partition_id = str(chunk_req.chunk.partition_id)
-                #    if partition_id not in self.partition_queues:
-                #        print(partition_id)
-                #        print(list(self.partition_queues.keys()))
-                #        raise ValueError(f"Partition {partition_id} does not exist in {list(self.partition_queues.keys())}")
-
-                #    # queue the chunk if it needs to be
-                #    if self.push_chunks[partition_id]:
-                #        self.partition_queues[partition_id].put(chunk_req)
-
-                #    print("listeners", self.partition_queues[partition_id].get_handles())
-                #    for handle in self.partition_queues[partition_id].get_handles():
-                #        print(self.operators[handle])
-
-                # Check self.completed queue for chunks which have been processed by all operators
-                # for partition, queue in self.completed.items():
-                #    for chunk_req in queue.get_all():
-                #        # unlink chunk that has finished processing
-                #        chunk_file_path = self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id)
-                #        chunk_file_path.unlink()
-                #        self.chunk_store.state_finish_upload(chunk_req.chunk.chunk_id)
-                #        logger.info(f"Finished processing chunk: {chunk_req.chunk.chunk_id}, partition: {chunk_req.chunk.partition_id}")
-
-                time.sleep(0.1)  # yield
-
         except Exception as e:
             self.error_queue.put(e)
             self.error_event.set()
             logger.error(f"[gateway_daemon] Exception in daemon loop: {e}")
             logger.exception(e)
 
         # shut down workers except for API to report status
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_daemon_api.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_daemon_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,186 +1,204 @@
 import logging
+from collections import defaultdict
 import logging.handlers
 import os
 import threading
-from collections import defaultdict
 from multiprocessing import Queue
+from multiprocessing.managers import DictProxy
 from queue import Empty
 from traceback import TracebackException
-from typing import Dict, List, Optional
-
+from typing import Dict, List, Tuple, Optional
+import json
 from flask import Flask, jsonify, request
 from werkzeug.serving import make_server
 
-from skyplane.broadcast.gateway.chunk_store import ChunkStore
-from skyplane.broadcast.gateway.operators.gateway_receiver import GatewayReceiver
 from skyplane.chunk import ChunkRequest, ChunkState
+from skyplane.gateway.chunk_store import ChunkStore
+from skyplane.gateway.operators.gateway_receiver import GatewayReceiver
 from skyplane.utils import logger
 
 
 class GatewayDaemonAPI(threading.Thread):
     """
     API documentation:
     * GET /api/v1/status - returns status of API
     * GET /api/v1/servers - returns list of running servers
     * POST /api/v1/servers - starts a new server
     * DELETE /api/v1/servers/<int:port> - stops a server
     * GET /api/v1/chunk_requests - returns list of chunk requests (use {'state': '<state>'} to filter)
-    * GET /api/v1/chunk_requests/<int:chunk_id> - returns chunk request
+    * GET /api/v1/chunk_requests/<chunk_id> - returns chunk request
     * POST /api/v1/chunk_requests - adds a new chunk request
-    * PUT /api/v1/chunk_requests/<int:chunk_id> - updates chunk request
+    * PUT /api/v1/chunk_requests/<chunk_id> - updates chunk request
     * GET /api/v1/chunk_status_log - returns list of chunk status log entries
+    * POST /api/v1/upload_id_maps - post a json which contains mapping of region:bucket:key to upload id to each server
     """
 
     def __init__(
         self,
         chunk_store: ChunkStore,
         gateway_receiver: GatewayReceiver,
         error_event,
         error_queue: Queue,
-        terminal_operators: Optional[Dict[str, List[str]]] = None,
+        terminal_operators: Dict[str, List[str]],
+        num_required_terminal: Dict[str, int],
+        upload_id_map: DictProxy,
         host="0.0.0.0",
         port=8081,
     ):
         super().__init__()
         self.app = Flask("gateway_metadata_server")
         self.chunk_store = chunk_store
         self.gateway_receiver = gateway_receiver
         self.error_event = error_event
         self.error_queue = error_queue
         self.terminal_operators = terminal_operators
+        self.num_required_terminal = num_required_terminal
         self.error_list: List[TracebackException] = []
         self.error_list_lock = threading.Lock()
+        self.upload_id_map = upload_id_map
 
         # load routes
         self.register_global_routes(self.app)
         self.register_server_routes(self.app)
         self.register_request_routes(self.app)
         self.register_error_routes(self.app)
         self.register_socket_profiling_routes(self.app)
 
         # make server
         self.host = host
         self.port = port
         self.url = "http://{}:{}".format(host, port)
 
         # chunk status log
+        self.state_update_lock = threading.Lock()
         self.chunk_status: Dict[int, str] = {}  # TODO: maintain as chunk_status_log is dumped
-        self.chunk_requests: Dict[int, ChunkRequest] = {}
-        self.sender_compressed_sizes: Dict = {}  # TODO: maintain as chunks are completed
+        self.chunk_requests: Dict[str, ChunkRequest] = {}
+        self.sender_compressed_sizes: Dict[str, Tuple[int, int]] = {}  # TODO: maintain as chunks are completed
         self.chunk_status_log: List[Dict] = []
-        self.chunk_status_log_lock = threading.Lock()
-
         self.chunk_completions = defaultdict(list)
 
         # socket profiles
+        # TODO: actually fill these out
         self.sender_socket_profiles: List[Dict] = []
         self.sender_socket_profiles_lock = threading.Lock()
         self.receiver_socket_profiles: List[Dict] = []
         self.receiver_socket_profiles_lock = threading.Lock()
 
-        logging.getLogger("werkzeug").setLevel(logging.WARNING)
+        logging.getLogger("werkzeug").setLevel(logging.DEBUG)
         self.server = make_server(host, port, self.app, threaded=True)
 
-    def pull_chunk_status_queue(self):
-        print("pulling queue")
-        out_events = []
-        while True:
-            try:
-                elem = self.chunk_store.chunk_status_queue.get_nowait()
-                print("status queue:", elem)
-                if elem["state"] == ChunkState.upload_complete.name:
-                    self.chunk_completions[elem["chunk_id"]].append(elem["state"])
+    def pull_chunk_status_queue(self, timeout=0.5):
+        with self.state_update_lock:
+            while True:
+                try:
+                    elem = self.chunk_store.chunk_status_queue.get(timeout=timeout)
+                except Empty:
+                    # print("[gateway_api] Chunk status queue empty, no more updates")
+                    break
 
+                handle = elem["handle"]
+                state = elem["state"]
                 chunk_id = elem["chunk_id"]
+                partition = elem["partition"]
+                chunk_file_path = self.chunk_store.get_chunk_file_path(elem["chunk_id"])
+
+                if chunk_id not in self.chunk_status:
+                    self.chunk_status[chunk_id] = ChunkState.registered.name
 
-                if self.chunk_status.get(elem["chunk_id"], None) != ChunkState.upload_complete.name and len(
-                    self.chunk_completions[elem["chunk_id"]]
-                ) == len(self.terminal_operators[elem["partition"]]):
-                    self.chunk_status[elem["chunk_id"]] = ChunkState.upload_complete.name
-                    print(
-                        f"chunk {chunk_id}: complete",
-                        elem["chunk_id"],
-                        "all operators have uploaded",
-                        len(self.terminal_operators[elem["partition"]]),
-                        self.terminal_operators,
-                    )
+                if self.chunk_status[chunk_id] == ChunkState.complete.name:
+                    assert not os.path.exists(chunk_file_path), f"Chunk path still exists even though completed {chunk_file_path}"
+                    continue
+
+                # if terminal operator, then mark a chunk completion
+                if handle in self.terminal_operators[elem["partition"]] and state == ChunkState.complete.name:
+                    self.chunk_completions[chunk_id].append(handle)
+
+                # if all terminal operators complete, then mark chunk complete
+                if (
+                    self.chunk_status.get(chunk_id, None) != ChunkState.complete.name
+                    and len(self.chunk_completions[chunk_id]) == self.num_required_terminal[partition]
+                ):
+                    # TODO: set this somewhere else
+                    self.chunk_status[chunk_id] = ChunkState.complete.name
+
+                    print(f"[gateway_api] chunk {chunk_id}: complete, all operators have uploaded {self.terminal_operators}")
                     # remove chunk file
-                    chunk_file_path = self.chunk_store.get_chunk_file_path(elem["chunk_id"])
                     if os.path.exists(chunk_file_path):
-                        print(f"chunk {chunk_id}: REMOVING FILE")
+                        logging.info(f"[gateway_api] Removing chunk file {chunk_file_path}")
                         chunk_file_path.unlink()
 
                     # record compressed size
-                    if "metadata" in elem and "compressed_size_bytes" in elem["metadata"]:
-                        self.sender_compressed_sizes[elem["chunk_id"]] = elem["metadata"]["compressed_size_bytes"]
+                    if "metadata" in elem and "compressed_size_bytes" in elem["metadata"] and "uncompressed_size_bytes" in elem["metadata"]:
+                        self.sender_compressed_sizes[chunk_id] = (
+                            elem["metadata"]["compressed_size_bytes"],
+                            elem["metadata"]["uncompressed_size_bytes"],
+                        )
                 else:
-                    if elem["state"] == ChunkState.upload_complete.name:
+                    if elem["state"] == ChunkState.complete.name:
                         print(
-                            f"chunk {chunk_id}: not complete",
-                            self.chunk_completions[elem["chunk_id"]],
-                            self.terminal_operators[elem["partition"]],
-                            elem["partition"],
+                            f"[gateway_api] After {handle}, chunk {chunk_id}, partition {partition}: not complete "
+                            + f"operators {self.chunk_completions[chunk_id]} have uploaded "
+                            + f"out of {self.terminal_operators}. "
+                            + f"Required completitions = {self.num_required_terminal[partition]}"
                         )
-                    else:
-                        print(f"chunk {chunk_id}: {elem['state']}")
 
-                out_events.append(elem)
-            except Empty:
-                break
+                    # else:
+                    #    print(f"[gateway_api] chunk {chunk_id}: after {handle} state = {elem['state']}")
 
-        self.chunk_status_log.extend(out_events)
+                # only update chunk status log with terminal operators
+                # otherwise, the client needs to filter chunk updates depending on whether the operator is terminal or not
+                # this would require us to inform the client about the terminal operators, whcih seems annoying (though doable)
+                # we can change this if we need to profile the chunk status progression through the DAG in detail
+                if elem["state"] == ChunkState.complete.name:
+                    if handle in self.terminal_operators[elem["partition"]]:
+                        self.chunk_status_log.append(elem)
+                else:
+                    self.chunk_status_log.append(elem)
 
     def run(self):
         self.server.serve_forever()
 
     def shutdown(self):
         self.server.shutdown()
 
     def register_global_routes(self, app):
-        # index route returns API version
         @app.route("/", methods=["GET"])
         def get_index():
             return jsonify({"version": "v1"})
 
-        # index for v1 api routes, return all available routes as HTML page with links
         @app.route("/api/v1", methods=["GET"])
         def get_v1_index():
             output = ""
             for rule in sorted(self.app.url_map.iter_rules(), key=lambda r: r.rule):
                 if rule.endpoint != "static":
                     methods = set(m for m in rule.methods if m not in ["HEAD", "OPTIONS"])
                     output += f"<a href='{rule.rule}'>{rule.rule}</a>: {methods}<br>"
             return output
 
-        # status route returns if API is up
         @app.route("/api/v1/status", methods=["GET"])
         def get_status():
             return jsonify({"status": "ok"})
 
-        # shutdown route
         @app.route("/api/v1/shutdown", methods=["POST"])
         def shutdown():
             self.shutdown()
             logger.error("Shutdown complete. Hard exit.")
             os._exit(1)
 
     def register_server_routes(self, app):
-        # list running gateway servers w/ ports
         @app.route("/api/v1/servers", methods=["GET"])
         def get_server_ports():
             return jsonify({"server_ports": self.gateway_receiver.server_ports})
 
-        # add a new server
         @app.route("/api/v1/servers", methods=["POST"])
         def add_server():
             new_port = self.gateway_receiver.start_server()
             return jsonify({"server_port": new_port})
 
-        # remove a server
         @app.route("/api/v1/servers/<int:port>", methods=["DELETE"])
         def remove_server(port: int):
             try:
                 self.gateway_receiver.stop_server(port)
                 return jsonify({"status": "ok"})
             except ValueError as e:
                 return jsonify({"error": str(e)}), 400
@@ -189,70 +207,79 @@
         def make_chunk_req_payload(chunk_req: ChunkRequest):
             state = self.chunk_status[chunk_req.chunk.chunk_id]
             state_name = state if state is not None else "unknown"
             return {"req": chunk_req.as_dict(), "state": state_name}
 
         def get_chunk_reqs(state=None) -> Dict[int, Dict]:
             out = {}
-            for chunk_id, chunk_state in self.chunk_status.items():
+            for chunk_id in list(self.chunk_status.keys()):
+                chunk_state = self.chunk_status[chunk_id]
                 if state is None or chunk_state == state:
-                    self.chunk_requests[chunk_id]
-                    out[chunk_id] = make_chunk_req_payload(chunk_id)
+                    chunk_req = self.chunk_requests[chunk_id]
+                    out[chunk_id] = make_chunk_req_payload(chunk_req)
             return out
 
         def add_chunk_req(body, state):
             if isinstance(body, dict):
-                self.chunk_store.add_chunk_request(ChunkRequest.from_dict(body), state)
-                return 1
-            elif isinstance(body, list):
-                for chunk_req in body:
-                    self.chunk_store.add_chunk_request(ChunkRequest.from_dict(chunk_req), state)
-                return len(body)
-
-        # list all chunk requests
-        # body json options:
-        #   if state is set in body, then filter by state
+                chunk_req = ChunkRequest.from_dict(body)
+                self.chunk_requests[chunk_req.chunk.chunk_id] = chunk_req
+                qsize, succ = self.chunk_store.add_chunk_request(chunk_req, state)
+                if not succ:
+                    return 0, qsize, False
+                return 1, qsize, True
+            else:
+                assert isinstance(body, list), f"Body must be list, got {type(body)}"
+                added = 0
+                for row in body:
+                    chunk_req = ChunkRequest.from_dict(row)
+                    self.chunk_requests[chunk_req.chunk.chunk_id] = chunk_req
+                    qsize, succ = self.chunk_store.add_chunk_request(chunk_req, state)
+                    if not succ:
+                        return added, qsize, False
+                    added += 1
+                return added, qsize, True
+
         @app.route("/api/v1/chunk_requests", methods=["GET"])
         def get_chunk_requests():
             state_param = request.args.get("state")
-            print("GOT REQUEST")
             if state_param is not None:
                 try:
                     state = ChunkState.from_str(state_param)
                 except ValueError:
                     return jsonify({"error": "invalid state"}), 400
                 return jsonify({"chunk_requests": get_chunk_reqs(state)})
             else:
                 return jsonify({"chunk_requests": get_chunk_reqs()})
 
         @app.route("/api/v1/incomplete_chunk_requests", methods=["GET"])
         def get_incomplete_chunk_requests():
-            return jsonify({"chunk_requests": {k: v for k, v in get_chunk_reqs().items() if v["state"] != "upload_complete"}})
+            return jsonify({"chunk_requests": {k: v for k, v in get_chunk_reqs().items() if v["state"] != "complete"}})
 
         # lookup chunk request given chunk worker_id
         @app.route("/api/v1/chunk_requests/<int:chunk_id>", methods=["GET"])
         def get_chunk_request(chunk_id: int):
             chunk_req = self.chunk_requests.get(chunk_id)
             if chunk_req:
                 return jsonify({"chunk_requests": [make_chunk_req_payload(chunk_req)]})
             else:
                 return jsonify({"error": f"Chunk {chunk_id} not found"}), 404
 
         # add a new chunk request with default state registered
         @app.route("/api/v1/chunk_requests", methods=["POST"])
         def add_chunk_request():
-            print("GOT CHUNK REQUEST", request.json)
+            print(f"[gateway_api] Recieved chunk request {request.json}")
             state_param = request.args.get("state", "registered")
-            n_added = add_chunk_req(request.json, ChunkState.from_str(state_param))
+            n_added, qsize, succ = add_chunk_req(request.json, ChunkState.from_str(state_param))
             # TODO: Add to chunk manager queue
-            return jsonify({"status": "ok", "n_added": n_added})
+            print(f"[gateway_api] Added {n_added} chunk requests to queue, size {qsize} success {succ}")
+            return jsonify({"status": succ, "n_added": n_added, "qsize": qsize})
 
         # update chunk request
-        @app.route("/api/v1/chunk_requests/<int:chunk_id>", methods=["PUT"])
-        def update_chunk_request(chunk_id: int):
+        @app.route("/api/v1/chunk_requests/<chunk_id>", methods=["PUT"])
+        def update_chunk_request(chunk_id: str):
             chunk_req = self.chunk_requests.get(chunk_id)
             if chunk_req is None:
                 return jsonify({"error": f"Chunk {chunk_id} not found"}), 404
             else:
                 if "state" in request.args:
                     try:
                         state = ChunkState.from_str(request.args.get("state"))
@@ -262,17 +289,32 @@
                     return jsonify({"status": "ok"})
                 else:
                     return jsonify({"error": "update not supported"}), 400
 
         # list chunk status log
         @app.route("/api/v1/chunk_status_log", methods=["GET"])
         def get_chunk_status_log():
-            with self.chunk_status_log_lock:  # TODO: why is this needed?
-                # self.chunk_status_log.extend(self.chunk_store.drain_chunk_status_queue())
-                return jsonify({"chunk_status_log": self.chunk_status_log})
+            n_entries = len(self.chunk_status_log)
+            status_log_copy = []  # copy to support concurrent access
+            for i in range(n_entries):
+                status_log_copy.append(self.chunk_status_log[i])
+            return jsonify({"chunk_status_log": status_log_copy})
+
+        # post the upload ids mapping
+        @app.route("/api/v1/upload_id_maps", methods=["POST"])
+        def update_upload_ids_mapping():
+            # TODO: beware that this assumes that only a single thread on the client is making requests
+            # if concurrent calls are made, this needs to be processed as chunk requests are
+            logging.debug(f"[gateway_api] Recieved id mapping request {request.json}")
+            # update upload id mapping
+            upload_ids = request.json
+            for region_tag in upload_ids.keys():
+                for key, upload_id in upload_ids[region_tag].items():
+                    self.upload_id_map[region_tag + key] = upload_id
+            return jsonify({"status": "ok"})
 
     def register_error_routes(self, app):
         @app.route("/api/v1/errors", methods=["GET"])
         def get_errors():
             with self.error_list_lock:
                 while True:
                     try:
@@ -295,18 +337,17 @@
                     except Empty:
                         break
                 return jsonify({"socket_profiles": self.receiver_socket_profiles})
 
         @app.route("/api/v1/profile/compression", methods=["GET"])
         def get_receiver_compression_profile():
             total_size_compressed_bytes, total_size_uncompressed_bytes = 0, 0
-            for k, v in self.sender_compressed_sizes.items():
-                total_size_compressed_bytes += v
-                # TODO: figure out how to get final size of chunks
-                total_size_uncompressed_bytes += self.chunk_requests[k].chunk.chunk_length_bytes
+            for _, (compressed_size, uncompressed_size) in self.sender_compressed_sizes.items():
+                total_size_compressed_bytes += compressed_size
+                total_size_uncompressed_bytes += uncompressed_size
             return jsonify(
                 {
                     "compressed_bytes_sent": total_size_compressed_bytes,
                     "uncompressed_bytes_sent": total_size_uncompressed_bytes,
                     "compression_ratio": total_size_uncompressed_bytes / total_size_compressed_bytes
                     if total_size_compressed_bytes > 0
                     else 0,
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/gateway_program.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/gateway_program.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from typing import Optional, List, Tuple
 import json
 from collections import defaultdict
-from typing import Optional, List
 
 
 class GatewayOperator:
     def __init__(self, op_type):
         self.op_type = op_type
         self.children = []
         self.handle = None
@@ -28,21 +28,30 @@
         return json.dumps(self.to_dict())
 
     def __repr__(self):
         return self.to_json()
 
 
 class GatewaySend(GatewayOperator):
-    def __init__(self, ip_address: str, region: str, num_connections: int = 32, compress: bool = False, encrypt: bool = False):
+    def __init__(
+        self,
+        target_gateway_id: str,
+        region: str,
+        num_connections: int = 32,
+        compress: bool = False,
+        encrypt: bool = False,
+        private_ip: bool = False,
+    ):
         super().__init__("send")
-        self.ip_address = ip_address
+        self.target_gateway_id = target_gateway_id  # gateway to send to
         self.region = region  # region to send to
         self.num_connections = num_connections  # default this for now
         self.compress = compress
         self.encrypt = encrypt
+        self.private_ip = private_ip  # whether to send to private or public IP (private for GCP->GCP)
 
 
 class GatewayReceive(GatewayOperator):
     def __init__(self, decompress: bool = False, decrypt: bool = False, max_pending_chunks: int = 1000):
         super().__init__("receive")
         self.decompress = decompress
         self.decrypt = decrypt
@@ -60,19 +69,20 @@
         super().__init__("read_object_store")
         self.bucket_name = bucket_name
         self.bucket_region = bucket_region
         self.num_connections = num_connections
 
 
 class GatewayWriteObjectStore(GatewayOperator):
-    def __init__(self, bucket_name: str, bucket_region: str, num_connections: int = 32):
+    def __init__(self, bucket_name: str, bucket_region: str, num_connections: int = 32, key_prefix: Optional[str] = ""):
         super().__init__("write_object_store")
         self.bucket_name = bucket_name
         self.bucket_region = bucket_region
         self.num_connections = num_connections
+        self.key_prefix = key_prefix
 
 
 class GatewayWriteLocal(GatewayOperator):
     def __init__(self, path: Optional[str] = None):
         super().__init__("write_local")
         self.path = path
 
@@ -90,37 +100,60 @@
 class GatewayProgram:
 
     """
     GatewayProgram is a class that defines the local topology for a gateway (i.e. how to handle chunks)
     We intend to extend GatewayProgram to eventually support operations on chunk data.
     """
 
+    ip_address = None
+
     def __init__(self):
         self._plan = defaultdict(list)
         self._ops = {}
 
-    def add_operators(self, ops: List[GatewayOperator], parent_op: Optional[GatewayOperator] = None, partition_id: Optional[str] = None):
+    def get_operators(self) -> List[GatewayOperator]:
+        return list(self._ops.values())
+
+    def add_operators(self, ops: List[GatewayOperator], parent_handle: Optional[str] = None, partition_id: Optional[str] = "default"):
+        parent_op = self._ops[parent_handle] if parent_handle else None
         ops_handles = []
         for op in ops:
             ops_handles.append(self.add_operator(op, parent_op, partition_id))
 
         return ops_handles
 
-    def add_operator(self, op: GatewayOperator, parent_op: Optional[GatewayOperator] = None, partition_id: Optional[str] = None):
+    def add_operator(self, op: GatewayOperator, parent_handle: Optional[str] = None, partition_id: Optional[str] = "default"):
+        parent_op = self._ops[parent_handle] if parent_handle else None
         if not parent_op:  # root operation
             self._plan[partition_id].append(op)
         else:
             parent_op.add_child(op)
         op.set_handle(f"operator_{len(list(self._ops.keys()))}")
         self._ops[op.handle] = op
         return op.handle
 
     def to_dict(self):
-        plan_dict = {}
+        """
+        Return dictionary representation of all partitions and gateway partitions.
+        Partitions with equivalent programs are grouped together to save space.
+        """
+        program_all = []
         for partition_id, op_list in self._plan.items():
-            plan_dict[partition_id] = []
+            # build gateway program representation
+            program = []
             for op in op_list:
-                plan_dict[partition_id].append(op.to_dict())
-        return plan_dict
+                program.append(op.to_dict())
+
+            # check if any existing
+            exists = False
+            for p in program_all:
+                if p["value"] == program:  # equivalent partition exists
+                    p["partitions"].append(partition_id)
+                    exists = True
+                    break
+            if not exists:
+                program_all.append({"value": program, "partitions": [partition_id]})
+
+        return program_all
 
     def to_json(self):
         return json.dumps(self.to_dict())
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/operators/gateway_operator.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/operators/gateway_operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import json
+from pathlib import Path
 import os
+from typing import List
 import queue
 import socket
 import ssl
 import time
 import traceback
-from abc import ABC, abstractmethod
 from functools import partial
-from multiprocessing import Event, Process
+from multiprocessing import Event, Process, Queue
+from multiprocessing.managers import DictProxy
 from typing import Dict, List, Optional
 
-import nacl.secret
 import urllib3
+import nacl.secret
+from abc import ABC, abstractmethod
 
-from skyplane.broadcast.gateway.chunk_store import ChunkStore
-from skyplane.broadcast.gateway.gateway_queue import GatewayQueue
-from skyplane.chunk import ChunkRequest
-from skyplane.chunk import ChunkState
 from skyplane.config_paths import cloud_config
-from skyplane.obj_store.object_store_interface import ObjectStoreInterface
-from skyplane.utils import logger
 from skyplane.utils.definitions import MB
+from skyplane.utils import logger
 from skyplane.utils.retry import retry_backoff
 from skyplane.utils.timer import Timer
+from skyplane.obj_store.object_store_interface import ObjectStoreInterface
+
+from skyplane.chunk import ChunkRequest, ChunkState
+from skyplane.gateway.gateway_queue import GatewayQueue
+from skyplane.gateway.chunk_store import ChunkStore
 
 
 class GatewayOperator(ABC):
     def __init__(
         self,
         handle: str,
         region: str,  # TODO: remove
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
+        error_queue: Queue,
         chunk_store: ChunkStore,
-        n_processes: int = 1,
+        n_processes: Optional[int] = 1,
     ):
         self.handle = handle
         self.region = region
         self.input_queue = input_queue
         self.output_queue = output_queue
         self.chunk_store = chunk_store
         self.error_event = error_event
@@ -68,86 +71,103 @@
     def stop_workers(self):
         for i in range(self.n_processes):
             self.exit_flags[i].set()
         for p in self.processes:
             p.join()
         self.processes = []
 
-    def worker_loop(self, worker_id: int, **kwargs):
+    def worker_loop(self, worker_id: int, *args):
         self.worker_id = worker_id
         while not self.exit_flags[worker_id].is_set() and not self.error_event.is_set():
             try:
                 # get chunk from input queue
                 try:
                     # will only get data for that handle
                     chunk_req = self.input_queue.get_nowait(self.handle)
                 except queue.Empty:
                     continue
 
+                # TODO: status logging
+                self.chunk_store.log_chunk_state(chunk_req, ChunkState.in_progress, operator_handle=self.handle, worker_id=worker_id)
                 # process chunk
-                succ = self.process(chunk_req, **kwargs)
+                succ = self.process(chunk_req, *args)
 
                 # place in output queue
                 if succ:
-                    print(f"{self.handle}: Placing chunk {chunk_req.chunk.chunk_id} in downstream queue", self.output_queue)
+                    self.chunk_store.log_chunk_state(chunk_req, ChunkState.complete, operator_handle=self.handle, worker_id=worker_id)
                     if self.output_queue is not None:
                         self.output_queue.put(chunk_req)
                     else:
-                        # mark completed
-                        print(f"{self.handle}: Marking chunk {chunk_req.chunk.chunk_id} as completed")
-                        self.chunk_store.log_chunk_state(chunk_req, ChunkState.upload_complete, metadata={"handle": self.handle})
+                        print(f"[{self.handle}:{self.worker_id}] Output queue is None - terminal operator")
+                    time.sleep(0.1)  # yield ?
                 else:
                     # failed to process - re-queue
-                    self.input_queue.put(chunk_req)
                     time.sleep(0.1)
+                    self.input_queue.put(chunk_req)
 
             except Exception as e:
-                logger.error(f"[sender:{self.worker_id}] Exception: {e}")
+                logger.error(f"[{self.handle}:{self.worker_id}] Exception: {e}")
                 self.error_queue.put(traceback.format_exc())
                 self.error_event.set()
                 self.exit_flags[worker_id].set()
 
         # run worker exit function
         self.worker_exit(worker_id)
 
     def worker_exit(self, worker_id: int):
         pass
 
     @abstractmethod
-    def process(self, chunk_req: ChunkRequest, **kwargs):
+    def process(self, chunk_req: ChunkRequest, **args):
         pass
 
 
 class GatewayWaitReciever(GatewayOperator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def process(self, chunk_req: ChunkRequest, **kwargs):
+    # TODO: alternative (potentially better performnace) implementation: connect via queue with GatewayReciever to listen
+    # for download completition events - join with chunk request queue from ChunkStore
+    def process(self, chunk_req: ChunkRequest):
         chunk_file_path = self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id)
         if not os.path.exists(chunk_file_path):  # chunk still not downloaded, re-queue
-            print("Chunk not downloaded yet, re-queueing", chunk_req.chunk.chunk_id, chunk_file_path)
+            # logger.debug(f"[{self.handle}:{self.worker_id}] Chunk {chunk_req.chunk.chunk_id} not downloaded yet, re-queueing")
             return False
+
+        # check to see if file is completed downloading
+        # Successfully recieved chunk 38400a29812142a486eaefcdebedf371, 161867776    0, 67108864
+        with open(chunk_file_path, "rb") as f:
+            data = f.read()
+            if len(data) < chunk_req.chunk.chunk_length_bytes:
+                # download not complete
+                return False
+            assert (
+                len(data) == chunk_req.chunk.chunk_length_bytes
+            ), f"Downloaded chunk length does not match expected length: {len(data)}, {chunk_req.chunk.chunk_length_bytes}"
+        print(
+            f"[{self.handle}:{self.worker_id}] Successfully recieved chunk {chunk_req.chunk.chunk_id}, {len(data)}, {chunk_req.chunk.chunk_length_bytes}"
+        )
         return True
 
 
 class GatewaySender(GatewayOperator):
     def __init__(
         self,
         handle: str,
         region: str,
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
+        error_queue: Queue,
         chunk_store: ChunkStore,
         ip_addr: str,
-        use_tls: bool = True,
-        use_compression: bool = True,
+        use_tls: Optional[bool] = True,
+        use_compression: Optional[bool] = True,
         e2ee_key_bytes: Optional[bytes] = None,
-        n_processes: int = 32,
+        n_processes: Optional[int] = 32,
     ):
         super().__init__(handle, region, input_queue, output_queue, error_event, error_queue, chunk_store, n_processes)
         self.ip_addr = ip_addr
         self.use_tls = use_tls
         self.use_compression = use_compression
         self.e2ee_key_bytes = e2ee_key_bytes
         self.args = (ip_addr,)
@@ -162,54 +182,61 @@
         if e2ee_key_bytes is None:
             self.e2ee_secretbox = None
         else:
             self.e2ee_secretbox = nacl.secret.SecretBox(e2ee_key_bytes)
 
         # SSL context
         if use_tls:
-            self.ssl_context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)  # type: ignore
+            self.ssl_context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
             self.ssl_context.check_hostname = False
             self.ssl_context.verify_mode = ssl.CERT_NONE
             logger.info(f"Using {str(ssl.OPENSSL_VERSION)}")
         else:
             self.ssl_context = None
 
         # process-local state
         self.sender_port: Optional[int] = None
         self.destination_ports: Dict[str, int] = {}  # ip_address -> int
         self.destination_sockets: Dict[str, socket.socket] = {}  # ip_address -> socket
         self.sent_chunk_ids: Dict[str, List[int]] = {}  # ip_address -> list of chunk_ids
-        self.http_pool = urllib3.PoolManager(retries=urllib3.Retry(total=3), cert_reqs="CERT_NONE")
+
+        # http pool
+        timeout = urllib3.util.Timeout(connect=10.0, read=None)  # no read timeout
+        self.http_pool = urllib3.PoolManager(retries=urllib3.Retry(total=3), cert_reqs="CERT_NONE", timeout=timeout)
 
     def worker_exit(self, worker_id: int):
         # close destination sockets
         logger.info(f"[sender:{worker_id}] exiting, closing sockets")
         for dst_socket in self.destination_sockets.values():
             dst_socket.close()
 
         # wait for all chunks to reach state "downloaded"
         # TODO: remove/replace for broadcast
         def wait_for_chunks():
             cr_status = {}
             for ip, ip_chunk_ids in self.sent_chunk_ids.items():
                 response = self.http_pool.request("GET", f"https://{ip}:8080/api/v1/incomplete_chunk_requests")
-                assert response.status == 200, f"{response.status_code} {response.data}"
+                assert response.status == 200, f"{response.status} {response.data}"
                 host_state = json.loads(response.data.decode("utf-8"))["chunk_requests"]
                 for chunk_id in ip_chunk_ids:
                     if chunk_id in host_state:
                         cr_status[chunk_id] = host_state[chunk_id]["state"]
             return all(status not in ["registered", "download_queued", "download_in_progress"] for status in cr_status.values())
 
         logger.info(f"[sender:{worker_id}] waiting for chunks to reach state 'downloaded'")
         wait_success = False
         for _ in range(60):
-            if wait_for_chunks():
-                wait_success = True
-                break
-            time.sleep(1)
+            try:
+                if wait_for_chunks():
+                    wait_success = True
+                    break
+            except Exception as e:
+                logger.error(f"[Gateway Sender wait_for_chunks()] Exception: {e}")
+
+            time.sleep(5)  # originally 1
         if not wait_success:
             raise Exception("Timed out waiting for chunks to reach state 'downloaded'")
         logger.info(f"[sender:{worker_id}] all chunks reached state 'downloaded'")
 
         # close servers
         logger.info(f"[sender:{worker_id}] exiting, closing servers")
         for dst_host, dst_port in self.destination_ports.items():
@@ -230,43 +257,66 @@
             sock = self.ssl_context.wrap_socket(sock)
             logger.info(f"[sender:{self.worker_id}] finished TLS handshake to {dst_host}:{self.destination_ports[dst_host]}")
         sock.settimeout(original_timeout)
         sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         return sock
 
     # send chunks to other instances
-    def process(self, chunk_req: ChunkRequest, dst_host: str, **kwargs):
+    def process(self, chunk_req: ChunkRequest, dst_host: str):
         """Send list of chunks to gateway server, pipelining small chunks together into a single socket stream."""
         # notify server of upcoming ChunkRequests
-        logger.debug(f"[sender:{self.worker_id}] Sending chunk ID {chunk_req.chunk.chunk_id} to IP {dst_host}")
+
+        # print(f"[{self.handle}:{self.worker_id}] Sending chunk ID {chunk_req.chunk.chunk_id} to IP {dst_host}")
+
+        # TODO: does this function need to be implemented to work for a list of chunks?
 
         chunk_ids = [chunk_req.chunk.chunk_id]
         chunk_reqs = [chunk_req]
-        print("sending!", chunk_ids)
-        # with Timer(f"prepare to pre-register chunks {chunk_ids} to {dst_host}"):
-        #    logger.debug(f"[sender:{self.worker_id}]:{chunk_ids} pre-registering chunks")
-        #    chunk_reqs = [self.chunk_store.get_chunk_request(chunk_id) for chunk_id in chunk_ids]
-        #    print("chunk  reqs", chunk_reqs)
-        with Timer(f"pre-register chunks {chunk_ids} to {dst_host}"):
-            register_body = json.dumps([c.as_dict() for c in chunk_reqs]).encode("utf-8")
-            print(register_body)
-            print("destination", f"https://{dst_host}:8080/api/v1/chunk_requests")
-            response = self.http_pool.request(
-                "POST", f"https://{dst_host}:8080/api/v1/chunk_requests", body=register_body, headers={"Content-Type": "application/json"}
-            )
-            assert response.status == 200 and json.loads(response.data.decode("utf-8")).get("status") == "ok"
-            logger.debug(f"[sender:{self.worker_id}]:{chunk_ids} registered chunks")
+        try:
+            with Timer(f"pre-register chunks {chunk_ids} to {dst_host}"):
+                # TODO: remove chunk request wrapper
+                # while True:
+                #   try:
+                #       response = self.http_pool.request(
+                #           "POST", f"https://{dst_host}:8080/api/v1/chunk_requests", body=register_body, headers={"Content-Type": "application/json"}
+                #       )
+                #       break
+                #   except Exception as e:
+                #       print("sender post error", e)
+                #       time.sleep(1)
+                n_added = 0
+                while n_added < len(chunk_reqs):
+                    register_body = json.dumps([c.chunk.as_dict() for c in chunk_reqs[n_added:]]).encode("utf-8")
+                    # print(f"[sender-{self.worker_id}]:{chunk_ids} register body {register_body}")
+                    response = self.http_pool.request(
+                        "POST",
+                        f"https://{dst_host}:8080/api/v1/chunk_requests",
+                        body=register_body,
+                        headers={"Content-Type": "application/json"},
+                    )
+                    reply_json = json.loads(response.data.decode("utf-8"))
+                    print(f"[sender-{self.worker_id}]", n_added, reply_json, dst_host)
+                    n_added += reply_json["n_added"]
+                    assert response.status == 200, f"Wrong response status {response.status}"
+                    # json.loads(response.data.decode("utf-8")).get("status") == "ok"
+                    if n_added == len(chunk_reqs):
+                        print(f"[sender-{self.worker_id}]:{chunk_ids} registered chunks")
+                    else:
+                        time.sleep(1)
+        except Exception as e:
+            print(f"[{self.handle}:{self.worker_id}] Error registering chunks {chunk_ids} to {dst_host}: {e}")
+            raise e
 
         # contact server to set up socket connection
         if self.destination_ports.get(dst_host) is None:
-            logger.debug(f"[sender:{self.worker_id}]:{chunk_ids} creating new socket")
+            print(f"[sender-{self.worker_id}]:{chunk_ids} creating new socket")
             self.destination_sockets[dst_host] = retry_backoff(
                 partial(self.make_socket, dst_host), max_retries=3, exception_class=socket.timeout
             )
-            logger.debug(f"[sender:{self.worker_id}]:{chunk_ids} created new socket")
+            print(f"[sender-{self.worker_id}]:{chunk_ids} created new socket")
         sock = self.destination_sockets[dst_host]
 
         # TODO: cleanup so this isn't a loop
         for idx, chunk_req in enumerate(chunk_reqs):
             # self.chunk_store.state_start_upload(chunk_id, f"sender:{self.worker_id}")
             chunk_id = chunk_req.chunk.chunk_id
             chunk = chunk_req.chunk
@@ -285,116 +335,108 @@
             #    compressed_length = wire_length
             # if self.e2ee_secretbox is not None and self.region == chunk_req.src_region:
             #    data = self.e2ee_secretbox.encrypt(data)
             #    wire_length = len(data)
 
             # send chunk header
             header = chunk.to_wire_header(n_chunks_left_on_socket=len(chunk_ids) - idx - 1, wire_length=wire_length, is_compressed=False)
-            logger.debug(f"[sender:{self.worker_id}]:{chunk_id} sending chunk header {header}")
+            # print(f"[sender-{self.worker_id}]:{chunk_id} sending chunk header {header}")
             header.to_socket(sock)
-            logger.debug(f"[sender:{self.worker_id}]:{chunk_id} sent chunk header")
+            # print(f"[sender-{self.worker_id}]:{chunk_id} sent chunk header")
 
             # send chunk data
             assert chunk_file_path.exists(), f"chunk file {chunk_file_path} does not exist"
             # file_size = os.path.getsize(chunk_file_path)
 
             with Timer() as t:
                 sock.sendall(data)
 
             # logger.debug(f"[sender:{self.worker_id}]:{chunk_id} sent at {chunk.chunk_length_bytes * 8 / t.elapsed / MB:.2f}Mbps")
-            logger.debug(f"[sender:{self.worker_id}]:{chunk_id} sent at {wire_length * 8 / t.elapsed / MB:.2f}Mbps")
+            print(f"[sender:{self.worker_id}]:{chunk_id} sent at {wire_length * 8 / t.elapsed / MB:.2f}Mbps")
 
             if dst_host not in self.sent_chunk_ids:
                 self.sent_chunk_ids[dst_host] = []
             self.sent_chunk_ids[dst_host].append(chunk_req.chunk.chunk_id)
 
         # success, so return true
-        print("Sending success!", chunk_req, dst_host)
         return True
 
 
 class GatewayRandomDataGen(GatewayOperator):
     def __init__(
         self,
         handle: str,
         region: str,
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
+        error_queue: Queue,
         chunk_store: ChunkStore,
         size_mb: int,
-        n_processes: int = 1,
+        n_processes: Optional[int] = 1,
     ):
         super().__init__(handle, region, input_queue, output_queue, error_event, error_queue, chunk_store, n_processes)
         self.size_mb = size_mb
 
-    def process(self, chunk_req: ChunkRequest, **kwargs):
+    def process(self, chunk_req: ChunkRequest):
         # wait until enough space available
         fpath = str(self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id).absolute())
         size_bytes = int(self.size_mb * MB)
         assert size_bytes > 0, f"Invalid size {size_bytes} for fallocate"
 
         while True:
             # create file with random data
             try:
                 os.system(f"fallocate -l {size_bytes} {fpath}")
                 file_size = os.path.getsize(fpath)
                 if file_size == size_bytes:
                     break
             except Exception:
-                logger.debug(f"[gen_data] Chunk store full, waiting before generating {chunk_req.chunk.chunk_id}")
+                print(f"[gen_data] Chunk store full, waiting before generating {chunk_req.chunk.chunk_id}")
                 time.sleep(0.1)
                 continue
 
-        # while self.chunk_store.remaining_bytes() < size_bytes * self.n_processes:
-        #    logger.debug(f"[gen_data] Chunk store full, waiting before generating {chunk_req.chunk.chunk_id}")
-        #    time.sleep(0.1)
-
-        # create file with random data
-        # os.system(f"fallocate -l {size_bytes} {fpath}")
-        # file_size = os.path.getsize(fpath)
-        # assert file_size == size_bytes, f"File {fpath} has size {file_size} but should be {size_bytes} - chunk store remaining size: {self.chunk_store.remaining_bytes()}"
-        print(f"Wrote chunk {chunk_req.chunk.chunk_id} to {fpath}")
+        logger.info(f"[{self.handle}:{self.worker_id}] Wrote chunk {chunk_req.chunk.chunk_id} with size {file_size} to {fpath}")
         chunk_req.chunk.chunk_length_bytes = os.path.getsize(fpath)
+
         return True
 
 
 class GatewayWriteLocal(GatewayOperator):
     def __init__(
         self,
         handle: str,
         region: str,
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
+        error_queue: Queue,
         chunk_store: ChunkStore,
         n_processes: int = 1,
     ):
         super().__init__(handle, region, input_queue, output_queue, error_event, error_queue, chunk_store, n_processes)
 
-    def process(self, chunk_req: ChunkRequest, **kwargs):
+    def process(self, chunk_req: ChunkRequest):
         # do nothing (already written locally)
         return True
 
 
 class GatewayObjStoreOperator(GatewayOperator):
     def __init__(
         self,
         handle: str,
         region: str,
+        bucket_name: str,
+        bucket_region: str,
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
-        n_processes: int = 1,
+        error_queue: Queue,
+        n_processes: Optional[int] = 1,
         chunk_store: Optional[ChunkStore] = None,
-        bucket_name: Optional[str] = None,
-        bucket_region: Optional[str] = None,
     ):
         super().__init__(handle, region, input_queue, output_queue, error_event, error_queue, chunk_store, n_processes)
         self.bucket_name = bucket_name
         self.bucket_region = bucket_region
         self.src_requester_pays = cloud_config.get_flag("requester_pays")
 
         # process-local state
@@ -414,51 +456,74 @@
 
 
 class GatewayObjStoreReadOperator(GatewayObjStoreOperator):
     def __init__(
         self,
         handle: str,
         region: str,
+        bucket_name: str,
+        bucket_region: str,
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
+        error_queue: Queue,
         n_processes: int = 32,
         chunk_store: Optional[ChunkStore] = None,
-        bucket_name: Optional[str] = None,
-        bucket_region: Optional[str] = None,
     ):
         super().__init__(
-            handle, region, input_queue, output_queue, error_event, error_queue, n_processes, chunk_store, bucket_name, bucket_region
+            handle, region, bucket_name, bucket_region, input_queue, output_queue, error_event, error_queue, n_processes, chunk_store
         )
 
     def process(self, chunk_req: ChunkRequest, **args):
-        print("reading", chunk_req.chunk.chunk_id, "key", chunk_req.chunk.src_key)
         fpath = str(self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id).absolute())
         # wait for free space
-        while self.chunk_store.remaining_bytes() < chunk_req.chunk.chunk_length_bytes * self.n_processes:
-            time.sleep(0.1)
-
-        logger.debug(f"[obj_store:{self.worker_id}] Start download {chunk_req.chunk.chunk_id} from {self.bucket_name}")
+        logger.debug(f"[{self.handle}:{self.worker_id}] Start download {chunk_req.chunk.chunk_id} from {self.bucket_name}")
 
         obj_store_interface = self.get_obj_store_interface(self.bucket_region, self.bucket_name)
 
         if self.src_requester_pays:
             obj_store_interface.set_requester_bool(True)
-        md5sum = retry_backoff(
-            partial(
-                obj_store_interface.download_object,
-                chunk_req.chunk.src_key,
-                fpath,
-                chunk_req.chunk.file_offset_bytes,
-                chunk_req.chunk.chunk_length_bytes,
-                generate_md5=True,
-            ),
-            max_retries=4,
-        )
+
+        # while self.chunk_store.remaining_bytes() < chunk_req.chunk.chunk_length_bytes * self.n_processes:
+        #    time.sleep(0.1)
+
+        # assert chunk_req.chunk.chunk_length_bytes > 0, f"Cannot have size 0 chunk {chunk_req.chunk}" # actually ok
+
+        if chunk_req.chunk.chunk_length_bytes == 0:
+            # nothing to do
+            # create empty file
+            Path(fpath).touch()
+            return True
+
+        while True:
+            # if self.chunk_store.remaining_bytes() < chunk_req.chunk.chunk_length_bytes * self.n_processes:
+            #    time.sleep(0.1)
+            #    continue
+            try:
+                md5sum = retry_backoff(
+                    partial(
+                        obj_store_interface.download_object,
+                        chunk_req.chunk.src_key,
+                        fpath,
+                        chunk_req.chunk.file_offset_bytes,
+                        chunk_req.chunk.chunk_length_bytes,
+                        generate_md5=True,
+                    ),
+                    max_retries=1,  # TODO: fix this - not a good solution
+                )
+
+                # ensure properly downloaded
+                file_size = os.path.getsize(fpath)
+                if file_size == chunk_req.chunk.chunk_length_bytes:
+                    break
+
+            except Exception as e:
+                logger.error(f"[obj_store:{self.worker_id}] Error reading key {chunk_req.chunk.src_key}: {str(e)}")
+                print(f"[obj_store:{self.worker_id}] Error reading key {chunk_req.chunk.src_key}: {str(e)}")
+                time.sleep(1)
 
         # update md5sum for chunk requests
         # TODO: create checksum operator
         # if not md5sum:
         #    logger.error(f"[obj_store:{self.worker_id}] Checksum was not generated for {chunk_req.chunk.src_key}")
         # else:
         #    self.chunk_store.update_chunk_checksum(chunk_req.chunk.chunk_id, md5sum)
@@ -472,41 +537,58 @@
 
 
 class GatewayObjStoreWriteOperator(GatewayObjStoreOperator):
     def __init__(
         self,
         handle: str,
         region: str,
+        bucket_name: str,
+        bucket_region: str,
         input_queue: GatewayQueue,
         output_queue: GatewayQueue,
         error_event,
-        error_queue: GatewayQueue,
-        n_processes: int = 32,
+        error_queue: Queue,
+        upload_id_map: DictProxy,  # map of upload_id mappings from client
+        n_processes: Optional[int] = 32,
         chunk_store: Optional[ChunkStore] = None,
-        bucket_name: Optional[str] = None,
-        bucket_region: Optional[str] = None,
+        prefix: Optional[str] = "",
     ):
         super().__init__(
-            handle, region, input_queue, output_queue, error_event, error_queue, n_processes, chunk_store, bucket_name, bucket_region
+            handle, region, bucket_name, bucket_region, input_queue, output_queue, error_event, error_queue, n_processes, chunk_store
         )
+        self.chunk_store = chunk_store
+        self.upload_id_map = upload_id_map
+        self.prefix = prefix
 
-    def process(self, chunk_req: ChunkRequest, **kwargs):
+    def process(self, chunk_req: ChunkRequest):
         fpath = str(self.chunk_store.get_chunk_file_path(chunk_req.chunk.chunk_id).absolute())
-        print("writing", chunk_req.chunk.dest_key, self.bucket_name, self.bucket_region, chunk_req.chunk.chunk_length_bytes)
         logger.debug(
-            f"[obj_store:{self.worker_id}] Start upload {chunk_req.chunk.chunk_id} to {self.bucket_name}, key {chunk_req.chunk.dest_key}"
+            f"[{self.handle}:{self.worker_id}] Start upload {chunk_req.chunk.chunk_id} to {self.bucket_name}, key {chunk_req.chunk.dest_key}"
         )
 
+        # TODO: cache object store interface
         obj_store_interface = self.get_obj_store_interface(self.bucket_region, self.bucket_name)
+
+        if chunk_req.chunk.multi_part:
+            upload_id_key = self.bucket_region + chunk_req.chunk.src_key  # format for upload id key
+            assert upload_id_key in self.upload_id_map, f"Upload id for {upload_id_key} not found {self.upload_id_map}"
+            upload_id = self.upload_id_map[upload_id_key]
+        else:
+            upload_id = None
+
+        key = self.prefix + chunk_req.chunk.dest_key
+        logger.debug(f"[obj_store:{self.worker_id}] Uploading to id {upload_id} for key {key} bucket {self.bucket_name}")
         retry_backoff(
             partial(
                 obj_store_interface.upload_object,
                 fpath,
-                chunk_req.chunk.dest_key,
+                key,
                 chunk_req.chunk.part_number,
-                chunk_req.chunk.upload_id,
+                upload_id,
                 check_md5=chunk_req.chunk.md5_hash,
             ),
-            max_retries=4,
+            max_retries=1,
+        )
+        logger.debug(
+            f"[obj_store:{self.worker_id}] Uploaded {chunk_req.chunk.chunk_id} partition {chunk_req.chunk.part_number} to {self.bucket_name}"
         )
-        logger.debug(f"[obj_store:{self.worker_id}] Uploaded {chunk_req.chunk.chunk_id} to {self.bucket_name}")
         return True
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/broadcast/gateway/operators/gateway_receiver.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/gateway/operators/gateway_receiver.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,43 +6,45 @@
 import traceback
 from contextlib import closing
 from multiprocessing import Event, Process, Value, Queue
 from typing import Optional, Tuple
 
 import nacl.secret
 
-from skyplane.broadcast.gateway.cert import generate_self_signed_certificate
-from skyplane.broadcast.gateway.chunk_store import ChunkStore
-from skyplane.chunk import WireProtocolHeader
-from skyplane.utils import logger
 from skyplane.utils.definitions import MB
+from skyplane.utils import logger
 from skyplane.utils.timer import Timer
 
+from skyplane.chunk import WireProtocolHeader
+from skyplane.gateway.cert import generate_self_signed_certificate
+from skyplane.gateway.chunk_store import ChunkStore
+
 
 class GatewayReceiver:
     def __init__(
         self,
         handle: str,
         region: str,
         chunk_store: ChunkStore,
         error_event,
         error_queue: Queue,
         recv_block_size=4 * MB,
         max_pending_chunks=1,
-        use_tls: bool = True,
-        use_compression: bool = True,
+        use_tls: Optional[bool] = True,
+        use_compression: Optional[bool] = True,
         e2ee_key_bytes: Optional[bytes] = None,
     ):
         self.handle = handle
         self.region = region
         self.chunk_store = chunk_store
         self.error_event = error_event
         self.error_queue = error_queue
         self.recv_block_size = recv_block_size
         self.max_pending_chunks = max_pending_chunks
+        print("Max pending chunks", self.max_pending_chunks)
         self.use_compression = use_compression
         if e2ee_key_bytes is None:
             self.e2ee_secretbox = None
         else:
             self.e2ee_secretbox = nacl.secret.SecretBox(e2ee_key_bytes)
         self.server_processes = []
         self.server_ports = []
@@ -61,22 +63,22 @@
             self.ssl_context = None
 
         # private state per worker
         self.worker_id: Optional[int] = None
 
     def start_server(self):
         started_event = Event()
-        port_value = Value("i", 0)
+        port = Value("i", 0)
 
         def server_worker(worker_id: int):
             self.worker_id = worker_id
             with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
                 sock.bind(("0.0.0.0", 0))
                 socket_port = sock.getsockname()[1]
-                port_value.value = socket_port  # type: ignore
+                port.value = socket_port  # type: ignore
                 exit_flag = Event()
 
                 def signal_handler(signal, frame):
                     exit_flag.set()
 
                 signal.signal(signal.SIGINT, signal_handler)
 
@@ -102,17 +104,17 @@
 
         gateway_id = self.next_gateway_worker_id
         self.next_gateway_worker_id += 1
         p = Process(target=server_worker, args=(gateway_id,))
         p.start()
         started_event.wait()
         self.server_processes.append(p)
-        self.server_ports.append(port_value.value)  # type: ignore
-        logger.info(f"[receiver:{port_value.value}] Started server)")  # type: ignore
-        return port_value.value  # type: ignore
+        self.server_ports.append(port.value)  # type: ignore
+        logger.info(f"[receiver:{port.value}] Started server)")  # type: ignore
+        return port.value  # type: ignore
 
     def stop_server(self, port: int):
         matched_process = None
         for server_port, server_process in zip(self.server_ports, self.server_processes):
             if server_port == port:
                 matched_process = server_process
                 break
@@ -135,38 +137,42 @@
 
     def stop_workers(self):
         self.stop_servers()
 
     def recv_chunks(self, conn: socket.socket, addr: Tuple[str, int]):
         server_port = conn.getsockname()[1]
         chunks_received = []
+        init_space = self.chunk_store.remaining_bytes()
+        print("Init space", init_space)
         while True:
             # receive header and write data to file
             logger.debug(f"[receiver:{server_port}] Blocking for next header")
             chunk_header = WireProtocolHeader.from_socket(conn)
             logger.debug(f"[receiver:{server_port}]:{chunk_header.chunk_id} Got chunk header {chunk_header}")
 
             # TODO: this wont work
             # chunk_request = self.chunk_store.get_chunk_request(chunk_header.chunk_id)
 
             # should_decrypt = self.e2ee_secretbox is not None and chunk_request.dst_region == self.region
             # should_decompress = chunk_header.is_compressed and chunk_request.dst_region == self.region
 
             # wait for space
-            # TODO: implement same fix as for gen_data
-            while self.chunk_store.remaining_bytes() < chunk_header.data_len * self.max_pending_chunks:
-                logger.debug(f"[reciever] Chunk store full, waiting before recieving more chunks")
-                time.sleep(0.1)
+            # while self.chunk_store.remaining_bytes() < chunk_header.data_len * self.max_pending_chunks:
+            #    print(
+            #        f"[receiver:{server_port}]: No remaining space with bytes {self.chunk_store.remaining_bytes()} data len {chunk_header.data_len} max pending {self.max_pending_chunks}, total space {init_space}"
+            #    )
+            #    time.sleep(0.1)
 
             # get data
             # self.chunk_store.state_queue_download(chunk_header.chunk_id)
             # self.chunk_store.state_start_download(chunk_header.chunk_id, f"receiver:{self.worker_id}")
             logger.debug(f"[receiver:{server_port}]:{chunk_header.chunk_id} wire header length {chunk_header.data_len}")
             with Timer() as t:
-                with self.chunk_store.get_chunk_file_path(chunk_header.chunk_id).open("wb") as f:
+                fpath = self.chunk_store.get_chunk_file_path(chunk_header.chunk_id)
+                with fpath.open("wb") as f:
                     socket_data_len = chunk_header.data_len
                     chunk_received_size = 0
                     to_write = bytearray(socket_data_len)
                     to_write_view = memoryview(to_write)
                     while socket_data_len > 0:
                         nbytes = conn.recv_into(to_write_view[chunk_received_size:], min(socket_data_len, self.recv_block_size))
                         socket_data_len -= nbytes
@@ -176,19 +182,41 @@
                                 receiver_id=self.worker_id,
                                 chunk_id=chunk_header.chunk_id,
                                 time_ms=t.elapsed * 1000.0,
                                 bytes=chunk_received_size,
                             )
                         )
                     to_write = bytes(to_write)
-                    f.write(to_write)
+
+                    # try to write data until successful
+                    while True:
+                        try:
+                            f.seek(0, 0)
+                            f.write(to_write)
+                            f.flush()
+
+                            # check size
+                            file_size = os.path.getsize(fpath)
+                            if file_size == chunk_header.data_len:
+                                break
+                            elif file_size >= chunk_header.data_len:
+                                raise ValueError(f"[Gateway] File size {file_size} greater than chunk size {chunk_header.data_len}")
+                        except Exception as e:
+                            print(e)
+
+                        print(
+                            f"[receiver:{server_port}]: No remaining space with bytes {self.chunk_store.remaining_bytes()} data len {chunk_header.data_len} max pending {self.max_pending_chunks}, total space {init_space}"
+                        )
+                        time.sleep(1)
             assert (
                 socket_data_len == 0 and chunk_received_size == chunk_header.data_len
             ), f"Size mismatch: got {chunk_received_size} expected {chunk_header.data_len} and had {socket_data_len} bytes remaining"
 
+            logger.debug(f"Recieved chunk {chunk_header.chunk_id} size {chunk_header.data_len}")
+
             # todo check hash
             # self.chunk_store.state_finish_download(chunk_header.chunk_id, f"receiver:{self.worker_id}")
             chunks_received.append(chunk_header.chunk_id)
 
             if chunk_header.n_chunks_left_on_socket == 0:
                 logger.debug(f"[receiver:{server_port}] End of stream reached")
                 return
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/chunk.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/chunk.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 class Chunk:
     """A Chunk is a contiguous piece of a file (a file may be one or more chunks)."""
 
     src_key: str  # human readable path where object is stored
     dest_key: str  # human readable path where object is stored
     chunk_id: str
     chunk_length_bytes: int
+    partition_id: Optional[str] = None  # for broadcast
     mime_type: Optional[str] = None
-    partition: Optional[str] = None
 
     # checksum
     md5_hash: Optional[bytes] = None  # 128 bits
 
     # multi-part upload/download info
+    multi_part: Optional[bool] = False
     file_offset_bytes: Optional[int] = None
     part_number: Optional[int] = None
-    upload_id: Optional[str] = None
+    upload_id: Optional[str] = None  # TODO: for broadcast, this is not used
 
     def to_wire_header(self, n_chunks_left_on_socket: int, wire_length: int, is_compressed: bool = False):
         return WireProtocolHeader(
             chunk_id=self.chunk_id, data_len=wire_length, is_compressed=is_compressed, n_chunks_left_on_socket=n_chunks_left_on_socket
         )
 
     def as_dict(self):
@@ -40,18 +41,18 @@
 
 # TODO: remove ChunkRequest abstraction (only need chunks)
 @dataclass
 class ChunkRequest:
     """A ChunkRequest stores all local state in the Gateway pertaining to a ChunkRequest."""
 
     chunk: Chunk
-    src_region: str
-    dst_region: str
-    src_type: str  # enum of {"object_store", "random", "read_local"}
-    dst_type: str  # enum of {"object_store", "save_local"}
+    src_region: Optional[str] = None
+    dst_region: Optional[str] = None
+    src_type: Optional[str] = None  # enum of {"object_store", "random", "read_local"}
+    dst_type: Optional[str] = None  # enum of {"object_store", "save_local"}
     src_random_size_mb: Optional[int] = None
     src_object_store_bucket: Optional[str] = None
     dst_object_store_bucket: Optional[str] = None
 
     def __post_init__(self):
         if self.src_type == "object_store":
             assert self.src_object_store_bucket is not None
@@ -63,28 +64,25 @@
     def as_dict(self):
         dict_out = asdict(self)
         dict_out["chunk"] = self.chunk.as_dict()
         return dict_out
 
     @staticmethod
     def from_dict(in_dict: Dict):
-        in_dict["chunk"] = Chunk.from_dict(in_dict["chunk"])
-        return ChunkRequest(**in_dict)
+        # in_dict["chunk"] = Chunk.from_dict(in_dict)
+        return ChunkRequest(**{"chunk": Chunk.from_dict(in_dict)})
 
 
 @total_ordering
 class ChunkState(Enum):
     registered = auto()
-    download_queued = auto()
-    download_in_progress = auto()
-    downloaded = auto()
-    upload_queued = auto()
-    upload_in_progress = auto()
-    upload_complete = auto()
+    in_progress = auto()
     failed = auto()
+    queued = auto()
+    complete = auto()
 
     @staticmethod
     def from_str(s: str):
         return ChunkState[s.lower()]
 
     def __lt__(self, other):
         return self.value < other.value
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from typing import Optional
 
 import typer
 from rich.prompt import IntPrompt
 
 import skyplane.cli.cli_cloud
 import skyplane.cli.cli_config
-import skyplane.cli.experiments
+
+# import skyplane.cli.experiments # disable experiments
 from skyplane import compute
+
 from skyplane.cli.cli_init import init
 from skyplane.cli.cli_transfer import cp, sync
 from skyplane.cli.impl.common import query_instances
 from skyplane.utils import logger
 from skyplane.utils.fn import do_parallel
 
 app = typer.Typer(name="skyplane")
@@ -24,15 +26,15 @@
     name="sync",
     help="Sync files between any two cloud object stores",
 )(sync)
 app.command(
     name="init",
     help="Initialize the Skyplane CLI with your cloud credentials",
 )(init)
-app.add_typer(skyplane.cli.experiments.app, name="experiments")
+# app.add_typer(skyplane.cli.experiments.app, name="experiments") # disable experiments
 app.add_typer(skyplane.cli.cli_cloud.app, name="cloud")
 app.add_typer(skyplane.cli.cli_config.app, name="config")
 
 
 @app.command()
 def deprovision(
     all: bool = typer.Option(False, "--all", "-a", help="Deprovision all resources including networks."),
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_cloud.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_cloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Cloud convenience interface
 """
 
 import json
+import uuid
 import subprocess
 import time
 from collections import defaultdict
 
 import typer
 from rich import print as rprint
 from typing import List
@@ -277,14 +278,46 @@
     # check skyplane AzureBlobInterface
     rprint(f"\n{hline}\n[bold]Checking Skyplane AzureBlobInterface[/bold]\n{hline}")
     from skyplane.obj_store.azure_blob_interface import AzureBlobInterface
 
     iface = AzureBlobInterface(account, container)
     print(iface.container_client.get_container_properties())
 
+    # write object temorarily
+    # check skyplane AzureBlobInterface
+    print(f"\n{hline}\n[bold]Checking Skyplane AzureBlobInterface[/bold]\n{hline}")
+    from skyplane.obj_store.azure_blob_interface import AzureBlobInterface
+
+    iface = AzureBlobInterface(account, container)
+    print(iface.container_client.get_container_properties())
+
+    # check if writeable
+    rprint(f"\n{hline}\n[bold]Checking Skyplane AzureBlobInterface write access[/bold]\n{hline}")
+    import tempfile
+    import random
+    import string
+
+    def generate_random_string(length):
+        """Generate a random string of given length"""
+        letters = string.ascii_letters
+        return "".join(random.choice(letters) for _ in range(length))
+
+    def create_temp_file(size):
+        """Create a temporary file with random data"""
+        with tempfile.NamedTemporaryFile(delete=False) as temp_file:
+            temp_file_path = temp_file.name
+            random_data = generate_random_string(size)
+            temp_file.write(random_data.encode())
+        return temp_file_path
+
+    tmp_file = create_temp_file(1024)
+    tmp_object = f"skyplane-{uuid.uuid4()}"
+    iface.upload_object(tmp_file, tmp_object)
+    iface.delete_objects([tmp_object])
+
 
 @app.command()
 def gcp_check(
     bucket: str = typer.Argument(..., help="GCP bucket to check access for"),
     debug: bool = typer.Option(False, "--debug", help="Print debug info"),
 ):
     hline = "=" * 80
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_config.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_init.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 import skyplane.api.usage
 from skyplane import compute
 from skyplane.cli.impl.common import print_header
 from skyplane.api.usage import UsageClient, UsageStatsStatus
 from skyplane.config import SkyplaneConfig
-from skyplane.config_paths import aws_config_path, gcp_config_path, config_path
+from skyplane.config_paths import aws_config_path, gcp_config_path, config_path, ibmcloud_config_path
 from skyplane.utils import logger
 
 
 def load_aws_config(config: SkyplaneConfig, non_interactive: bool = False) -> SkyplaneConfig:
     try:
         import boto3
     except ImportError:
         config.aws_enabled = False
-        typer.secho("    AWS support disabled because boto3 is not installed. Run `pip install skyplane[aws].`", fg="red", err=True)
+        typer.secho("    AWS support disabled because boto3 is not installed. Run `pip install 'skyplane[aws]'`.", fg="red", err=True)
         return config
     if non_interactive or typer.confirm("    Do you want to configure AWS support in Skyplane?", default=True):
         session = boto3.Session()
         credentials_session = session.get_credentials()
         if credentials_session is None:
             config.aws_enabled = False
         else:
@@ -59,14 +59,24 @@
             return config
     else:
         config.aws_enabled = False
         typer.secho("    Disabling AWS support", fg="blue")
         return config
 
 
+def load_cloudflare_config(config: SkyplaneConfig, non_interactive: bool = False) -> SkyplaneConfig:
+    if non_interactive or typer.confirm("    Do you want to configure Cloudflare support in Skyplane?", default=True):
+        config.cloudflare_access_key_id = typer.prompt("    Enter the R2 access key ID")
+        config.cloudflare_secret_access_key = typer.prompt("    Enter the R2 secret access key")
+    else:
+        config.cloudflare_enabled = False
+        typer.secho("    Disabling Cloudflare support", fg="blue")
+    return config
+
+
 def load_azure_config(config: SkyplaneConfig, force_init: bool = False, non_interactive: bool = False) -> SkyplaneConfig:
     def clear_azure_config(config, verbose=True):
         if verbose:
             typer.secho("    Disabling Azure support", fg="blue")
         config.azure_subscription_id = None
         config.azure_client_id = None
         config.azure_principal_id = None
@@ -76,20 +86,21 @@
     def make_role_cmds(principal_id, subscription_id):
         roles = ["Contributor", "Storage Blob Data Contributor", "Storage Account Contributor"]
         return [
             "az role assignment create --role".split(" ")
             + [role]
             + f"--assignee-object-id {principal_id} --assignee-principal-type ServicePrincipal".split(" ")
             + f"--subscription {subscription_id}".split(" ")
+            + f"--scope /subscriptions/{subscription_id}".split(" ")
             for role in roles
         ]
 
-    def run_az_cmd(cmd: List[str]):
+    def run_az_cmd(cmd: List[str], ignore_error=False):
         out, err = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()
-        if err:
+        if err and not ignore_error:
             typer.secho(f"    Error running command: {cmd}", fg="red", err=True)
             typer.secho(f"    stdout: {out.decode('utf-8')}", fg="red", err=True)
             typer.secho(f"    stderr: {err.decode('utf-8')}", fg="red", err=True)
             return False, out, err
         return True, out, err
 
     if non_interactive or typer.confirm("    Do you want to configure Azure support in Skyplane?", default=True):
@@ -202,26 +213,31 @@
                     "    Enter the name for the user managed identity that Skyplane VMs will use to access your Azure Storage Accounts (the default should work in most cases)",
                     default=defaults["umi_name"],
                 )
                 if not non_interactive
                 else defaults["umi_name"]
             )
 
+        enable_quota_provider_cmd = f"az provider register -n Microsoft.Quota"
         change_subscription_cmd = f"az account set --subscription {config.azure_subscription_id}"
         create_rg_cmd = f"az group create -l westus2 -n {config.azure_resource_group}"
         create_umi_cmd = f"az identity create -g {config.azure_resource_group} -n {config.azure_umi_name}"
         typer.secho(f"    I will run the following commands to create an Azure managed identity:", fg="blue")
+        typer.secho(f"        $ {enable_quota_provider_cmd}", fg="yellow")
         typer.secho(f"        $ {change_subscription_cmd}", fg="yellow")
         typer.secho(f"        $ {create_rg_cmd}", fg="yellow")
         typer.secho(f"        $ {create_umi_cmd}", fg="yellow")
 
         with Progress(
             TextColumn("    "), SpinnerColumn(), TextColumn("Creating Skyplane managed identity{task.description}"), transient=True
         ) as progress:
             progress.add_task("", total=None)
+            # NOTE: we want to run this command early on because it takes time to register the quota provider
+            _ = run_az_cmd(enable_quota_provider_cmd.split(), ignore_error=True)
+
             cmd_success, out, err = run_az_cmd(change_subscription_cmd.split())
             if not cmd_success:
                 return clear_azure_config(config)
             cmd_success, out, err = run_az_cmd(create_rg_cmd.split())
             if not cmd_success:
                 return clear_azure_config(config)
             cmd_success, out, err = run_az_cmd(create_umi_cmd.split())
@@ -324,15 +340,15 @@
         inferred_cred, inferred_project = compute.GCPAuthentication.get_adc_credential()
         if inferred_cred is None:  # or inferred_project is None:
             typer.secho("    Default GCP credentials are not set up yet. Run `gcloud auth application-default login`.", fg="red", err=True)
             typer.secho("    https://cloud.google.com/docs/authentication/getting-started", fg="red", err=True)
             return disable_gcp_support()
         else:
             typer.secho("    GCP credentials found in GCP CLI", fg="blue")
-            if non_interactive or typer.confirm("    GCP credentials found, do you want to enable GCP support in Skyplane?", default=True):
+            if non_interactive or typer.confirm("    Do you want to enable GCP support in Skyplane?", default=True):
                 if not non_interactive:
                     config.gcp_project_id = typer.prompt("    Enter the GCP project ID", default=inferred_project)
 
                 else:
                     config.gcp_project_id = inferred_project
                 assert config.gcp_project_id is not None, "GCP project ID must not be None"
                 config.gcp_enabled = True
@@ -349,56 +365,163 @@
                 return config
             else:
                 return disable_gcp_support()
     else:
         return disable_gcp_support()
 
 
+def load_ibmcloud_config(config: SkyplaneConfig, force_init: bool = False, non_interactive: bool = False) -> SkyplaneConfig:
+    try:
+        HOME_DIR = os.path.expanduser("~")
+        CONFIG_DIR = os.path.join(HOME_DIR, ".bluemix")
+        CONFIG_FILE = os.path.join(CONFIG_DIR, "ibm_credentials")
+
+        def load_yaml_config(config_filename):
+            import yaml
+
+            try:
+                with open(config_filename, "r") as config_file:
+                    data = yaml.safe_load(config_file)
+            except FileNotFoundError:
+                data = {}
+
+            return data
+
+        def get_default_config_filename():
+            """
+            First checks .ibm_config
+            then checks IBM_CONFIG_FILE environment variable
+            then ~/.ibm/config
+            """
+            if "IBM_CONFIG_FILE" in os.environ:
+                config_filename = os.environ["IBM_CONFIG_FILE"]
+
+            elif os.path.exists(".ibm_config"):
+                config_filename = os.path.abspath(".ibm_credentials")
+
+            else:
+                config_filename = CONFIG_FILE
+                if not os.path.exists(config_filename):
+                    return None
+
+            return config_filename
+
+        def load_config():
+            """Load the configuration"""
+            config_data = None
+            config_filename = get_default_config_filename()
+            if config_filename:
+                config_data = load_yaml_config(config_filename)
+            else:
+                # throw exception
+                raise Exception(f"IBM Config file not foud in {config_filename}")
+
+            return config_data
+
+    except ImportError:
+        config.ibmcloud_enabled = False
+        typer.secho(
+            "    IBM Cloud support disabled because ibm_boto3 is not installed. Run `pip install skyplane[ibmcloud].`", fg="red", err=True
+        )
+        return config
+    if non_interactive or typer.confirm("    Do you want to configure IBM Cloud support in Skyplane?", default=True):
+        ibm_config = load_config()
+        config.ibmcloud_useragent = ibm_config["user_agent"] if "user_agent" in ibm_config else "skyplane-ibm"
+
+        if "iam" in ibm_config and "ibm_iam_key" in ibm_config["iam"]:
+            config.ibmcloud_iam_key = ibm_config["iam"].get("ibm_iam_key")
+
+        if "iam" in ibm_config and "iam_endpoint" in ibm_config["iam"]:
+            config.ibmcloud_iam_endpoint = ibm_config["iam"].get("iam_endpoint")
+        else:
+            config.ibmcloud_iam_endpoint = "https://iam.cloud.ibm.com"
+
+        if "cos" in ibm_config and "access_key" in ibm_config["cos"]:
+            config.ibmcloud_access_id = ibm_config["cos"]["access_key"]
+
+        if "cos" in ibm_config and "secret_key" in ibm_config["cos"]:
+            config.ibmcloud_secret_key = ibm_config["cos"]["secret_key"]
+
+        if "ibm" in ibm_config and "resource_group_id" in ibm_config["ibm"]:
+            config.ibmcloud_resource_group_id = ibm_config["ibm"]["resource_group_id"]
+
+        if config.ibmcloud_access_id is not None:
+            config.ibmcloud_enabled = True
+
+        auth = compute.IBMCloudAuthentication(config=config)
+        if config.ibmcloud_enabled:
+            typer.secho(f"    Loaded IBM Cloud credentials ", fg="blue")
+            config.ibmcloud_enabled = True
+            auth.save_region_config(config)
+            typer.secho(f"    IBM Cloud  config file saved to {ibmcloud_config_path}", fg="blue")
+            return config
+        else:
+            typer.secho(f"    COS credentials not found {get_default_config_filename()}", fg="red", err=True)
+            typer.secho("    Disabling IBM Cloud support", fg="blue")
+            if auth is not None:
+                auth.clear_region_config()
+            return config
+    else:
+        config.cos_enabled = False
+        typer.secho("    Disabling IBM Cloud support", fg="blue")
+        return config
+
+
 def init(
     non_interactive: bool = typer.Option(False, "--non-interactive", "-y", help="Run non-interactively"),
     reinit_azure: bool = False,
     reinit_gcp: bool = False,
+    reinit_ibm: bool = False,
+    reinit_cloudflare: bool = False,
     disable_config_aws: bool = False,
     disable_config_azure: bool = False,
     disable_config_gcp: bool = False,
+    disable_config_ibm: bool = True,  # TODO: eventuall enable IBM
+    disable_config_cloudflare: bool = False,
 ):
     """
     It loads the configuration file, and if it doesn't exist, it creates a default one. Then it creates
-    AWS, Azure, and GCP region list configurations.
+    AWS, Azure, IBM and GCP region list configurations.
 
     :param reinit_azure: If true, will reinitialize the Azure region list and credentials
     :type reinit_azure: bool
     :param reinit_gcp: If true, will reinitialize the GCP region list and credentials
     :type reinit_gcp: bool
+    :param reinit_ibm: If true, will reinitialize the IBM Cloud region list and credentials
+    :type reinit_ibm: bool
     :param disable_config_aws: If true, will disable AWS configuration (may still be enabled if environment variables are set)
     :type disable_config_aws: bool
     :param disable_config_azure: If true, will disable Azure configuration (may still be enabled if environment variables are set)
     :type disable_config_azure: bool
     :param disable_config_gcp: If true, will disable GCP configuration (may still be enabled if environment variables are set)
     :type disable_config_gcp: bool
+    :param disable_config_ibm: If true, will disable IBM Cloud configuration (may still be enabled if environment variables are set)
+    :type disable_config_ibm: bool
+    :param disable_config_cloudflare: If true, will disable Cloudflare configuration (may still be enabled if environment variables are set)
+    :type disable_config_cloudflare: bool
     """
     print_header()
 
     if non_interactive:
         logger.warning("Non-interactive mode enabled. Automatically confirming interactive questions.")
 
     if config_path.exists():
         logger.debug(f"Found existing configuration file at {config_path}, loading")
         cloud_config = SkyplaneConfig.load_config(config_path)
     else:
         cloud_config = SkyplaneConfig.default_config()
 
     # load AWS config
-    if not (reinit_azure or reinit_gcp):
-        typer.secho("\n(1) Configuring AWS:", fg="yellow", bold=True)
+    if not (reinit_azure or reinit_gcp or reinit_ibm):
+        typer.secho("\n(1) configuring AWS:", fg="yellow", bold=True)
         if not disable_config_aws:
             cloud_config = load_aws_config(cloud_config, non_interactive=non_interactive)
 
     # load Azure config
-    if not reinit_gcp:
+    if not (reinit_gcp or reinit_ibm):
         if reinit_azure:
             typer.secho("\nConfiguring Azure:", fg="yellow", bold=True)
         else:
             typer.secho("\n(2) Configuring Azure:", fg="yellow", bold=True)
         if not disable_config_azure:
             cloud_config = load_azure_config(cloud_config, force_init=reinit_azure, non_interactive=non_interactive)
 
@@ -407,14 +530,27 @@
         if reinit_gcp:
             typer.secho("\nConfiguring GCP:", fg="yellow", bold=True)
         else:
             typer.secho("\n(3) Configuring GCP:", fg="yellow", bold=True)
         if not disable_config_gcp:
             cloud_config = load_gcp_config(cloud_config, force_init=reinit_gcp, non_interactive=non_interactive)
 
+    # load cloudflare config
+    if not reinit_cloudflare and not disable_config_cloudflare:  # TODO: fix reinit logic
+        typer.secho("\n(4) Configuring Cloudflare R2:", fg="yellow", bold=True)
+        if not disable_config_cloudflare:
+            cloud_config = load_cloudflare_config(cloud_config, non_interactive=non_interactive)
+
+    # load IBMCloud config
+    if not disable_config_ibm and not reinit_ibm:
+        # TODO: fix IBM configuration to not fail on file finding
+        typer.secho("\n(4) Configuring IBM Cloud:", fg="yellow", bold=True)
+        if not disable_config_ibm:
+            cloud_config = load_ibmcloud_config(cloud_config, force_init=reinit_ibm, non_interactive=non_interactive)
+
     cloud_config.to_config_file(config_path)
     typer.secho(f"\nConfig file saved to {config_path}", fg="green")
 
     # Set metrics collection by default
     usage_stats_var = UsageClient.usage_stats_status()
     if usage_stats_var is UsageStatsStatus.DISABLED_EXPLICITLY:
         rprint(skyplane.api.usage.USAGE_STATS_DISABLED_MESSAGE)
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/cli_transfer.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/cli_transfer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import os
 import signal
-import sys
 import time
 import traceback
 from dataclasses import dataclass
 from typing import Dict, Any, Optional, List
 
 import typer
 from rich.progress import Progress, TextColumn, SpinnerColumn
 
 import skyplane
-from skyplane.api.config import TransferConfig, AWSConfig, GCPConfig, AzureConfig
-from skyplane.api.transfer_job import CopyJob
+from skyplane.api.config import TransferConfig, AWSConfig, GCPConfig, AzureConfig, IBMCloudConfig
+from skyplane.api.transfer_job import CopyJob, SyncJob, TransferJob
 from skyplane.cli.impl.cp_replicate_fallback import (
     replicate_onprem_cp_cmd,
     replicate_onprem_sync_cmd,
     replicate_small_cp_cmd,
     replicate_small_sync_cmd,
 )
 from skyplane.cli.impl.common import print_header, console, print_stats_completed, register_exception_handler
 from skyplane.api.usage import UsageClient
 from skyplane.config import SkyplaneConfig
 from skyplane.config_paths import cloud_config, config_path
-from skyplane.obj_store.object_store_interface import ObjectStoreInterface
+from skyplane.obj_store.object_store_interface import ObjectStoreInterface, StorageInterface
+from skyplane.obj_store.file_system_interface import FileSystemInterface
 from skyplane.cli.impl.progress_bar import ProgressBarTransferHook
 from skyplane.utils import logger
 from skyplane.utils.definitions import GB, format_bytes
-from skyplane.utils.fn import do_parallel
 from skyplane.utils.path import parse_path
 
 
 @dataclass
 class TransferStats:
     monitor_status: str
     total_runtime_s: Optional[float] = None
@@ -50,42 +49,62 @@
         }
 
 
 class SkyplaneCLI:
     def __init__(self, src_region_tag: str, dst_region_tag: str, args: Dict[str, Any], skyplane_config: Optional[SkyplaneConfig] = None):
         self.src_region_tag, self.dst_region_tag = src_region_tag, dst_region_tag
         self.args = args
-        self.aws_config, self.azure_config, self.gcp_config = self.to_api_config(skyplane_config or cloud_config)
+        self.aws_config, self.azure_config, self.gcp_config, self.ibmcloud_config = self.to_api_config(skyplane_config or cloud_config)
+
+        # update config
+        # TODO: set remaining config params
+        if skyplane_config:
+            skyplane_config.set_flag("multipart_enabled", str(self.args["multipart"]))
+        if cloud_config:
+            cloud_config.set_flag("multipart_enabled", str(self.args["multipart"]))
+
         self.transfer_config = self.make_transfer_config(skyplane_config or cloud_config)
         self.client = skyplane.SkyplaneClient(
-            aws_config=self.aws_config, azure_config=self.azure_config, gcp_config=self.gcp_config, transfer_config=self.transfer_config
+            aws_config=self.aws_config,
+            azure_config=self.azure_config,
+            gcp_config=self.gcp_config,
+            transfer_config=self.transfer_config,
+            ibmcloud_config=self.ibmcloud_config,
         )
         typer.secho(f"Using Skyplane version {skyplane.__version__}", fg="bright_black")
-        typer.secho(f"Logging to: {self.client.log_dir / 'client.log'}", fg="bright_black")
 
     def to_api_config(self, config: SkyplaneConfig):
         aws_config = AWSConfig(aws_enabled=config.aws_enabled)
         # todo: fix azure config support by collecting azure umi name and resource group and store in skyplane config
         gcp_config = GCPConfig(gcp_project_id=config.gcp_project_id, gcp_enabled=config.gcp_enabled)
+        ibmcloud_config = IBMCloudConfig(
+            ibmcloud_access_id=config.ibmcloud_access_id,
+            ibmcloud_secret_key=config.ibmcloud_secret_key,
+            ibmcloud_iam_key=config.ibmcloud_iam_key,
+            ibmcloud_iam_endpoint=config.ibmcloud_iam_endpoint,
+            ibmcloud_useragent=config.ibmcloud_useragent,
+            ibmcloud_resource_group_id=config.ibmcloud_resource_group_id,
+            ibmcloud_enabled=config.ibmcloud_enabled,
+        )
         if not config.azure_resource_group or not config.azure_umi_name:
             typer.secho(
                 "Azure resource group and UMI name not configured correctly. Please reinit Azure with `skyplane init --reinit-azure`.",
                 fg=typer.colors.RED,
                 err=True,
             )
-            return aws_config, None, gcp_config
+            return aws_config, None, gcp_config, ibmcloud_config
         azure_config = AzureConfig(
             config.azure_subscription_id,
             config.azure_resource_group,
             config.azure_principal_id,
             config.azure_umi_name,
             config.azure_client_id,
             config.azure_enabled,
         )
-        return aws_config, azure_config, gcp_config
+        return aws_config, azure_config, gcp_config, ibmcloud_config
 
     def make_transfer_config(self, config: SkyplaneConfig) -> TransferConfig:
         intraregion = self.src_region_tag == self.dst_region_tag
         return TransferConfig(
             autoterminate_minutes=config.get_flag("autoshutdown_minutes"),
             requester_pays=config.get_flag("requester_pays"),
             use_bbr=config.get_flag("bbr"),
@@ -94,14 +113,15 @@
             use_socket_tls=config.get_flag("encrypt_socket_tls") if not intraregion else False,
             aws_use_spot_instances=config.get_flag("aws_use_spot_instances"),
             azure_use_spot_instances=config.get_flag("azure_use_spot_instances"),
             gcp_use_spot_instances=config.get_flag("gcp_use_spot_instances"),
             aws_instance_class=config.get_flag("aws_instance_class"),
             azure_instance_class=config.get_flag("azure_instance_class"),
             gcp_instance_class=config.get_flag("gcp_instance_class"),
+            ibmcloud_instance_class=config.get_flag("ibmcloud_instance_class"),
             gcp_use_premium_network=config.get_flag("gcp_use_premium_network"),
             multipart_enabled=config.get_flag("multipart_enabled"),
             multipart_threshold_mb=config.get_flag("multipart_min_threshold_mb"),
             multipart_chunk_size_mb=config.get_flag("multipart_chunk_size_mb"),
             multipart_max_chunks=config.get_flag("multipart_max_chunks"),
         )
 
@@ -162,33 +182,52 @@
             typer.secho(f"Transfer is small enough to delegate to native tools. Delegating to: {small_transfer_cmd}", fg="yellow")
             typer.secho(f"You can disable this with `skyplane config set native_cmd_enabled false`", fg="bright_black")
             os.system(small_transfer_cmd)
             return True
         else:
             return False
 
-    def make_dataplane(self, **solver_args) -> skyplane.Dataplane:
-        dp = self.client.dataplane(*self.src_region_tag.split(":"), *self.dst_region_tag.split(":"), **solver_args)
-        logger.fs.debug(f"Using dataplane: {dp}")
-        return dp
-
-    def confirm_transfer(self, dp: skyplane.Dataplane, query_n: int = 5, ask_to_confirm_transfer=True) -> bool:
+    # def make_dataplane(self, **solver_args) -> skyplane.Dataplane:
+    #    if self.src_region_tag.split(":")[0] == "hdfs":
+    #        self.src_region_tag = self.dst_region_tag
+    #    dp = self.client.dataplane(*self.src_region_tag.split(":"), *self.dst_region_tag.split(":"), **solver_args)
+    #    logger.fs.debug(f"Using dataplane: {dp}")
+    #    return dp
+
+    def make_pipeline(self, **solver_args) -> skyplane.Pipeline:
+        pipeline = self.client.pipeline(**solver_args)
+        logger.fs.debug(f"Using pipeline: {pipeline}")
+        return pipeline
+
+    def confirm_transfer(
+        self, pipeline: skyplane.Pipeline, src_region_tag: str, dest_region_tags: List[str], query_n: int = 5, ask_to_confirm_transfer=True
+    ) -> bool:
         """Prompts the user to confirm their transfer by querying the first query_n files from the TransferJob"""
-        if not len(dp.jobs_to_dispatch) > 0:
+        if not len(pipeline.jobs_to_dispatch) > 0:
             typer.secho("No jobs to dispatch.")
             return False
-        transfer_pair_gen = dp.jobs_to_dispatch[0].gen_transfer_pairs()  # type: ignore
-        console.print(f"[bold yellow]Will transfer objects from {dp.src_region_tag} to {dp.dst_region_tag}[/bold yellow]")
-        sorted_counts = sorted(dp.topology.per_region_count().items(), key=lambda x: x[0])
+        transfer_pair_gen = pipeline.jobs_to_dispatch[0].gen_transfer_pairs()  # type: ignore
+        if len(dest_region_tags) == 1:
+            console.print(f"[bold yellow]Will transfer objects from {src_region_tag} to {dest_region_tags[0]}[/bold yellow]")
+        else:
+            console.print(f"[bold yellow]Will transfer objects from {src_region_tag} to {dest_region_tags}[/bold yellow]")
+
+        if src_region_tag.startswith("local") or dest_region_tags[0].startswith("local"):
+            # TODO: should still pass cost estimate
+            console.print(f"[yellow]Note: local transfers are not monitored by Skyplane[yellow]")
+            return True
+
+        topology = pipeline.planner.plan(pipeline.jobs_to_dispatch)
+        sorted_counts = sorted(topology.per_region_count().items(), key=lambda x: x[0])
         console.print(
             f"  [bold][blue]VMs to provision:[/blue][/bold] [bright_black]{', '.join(f'{c}x {r}' for r, c in sorted_counts)}[/bright_black]"
         )
-        if dp.topology.cost_per_gb:
+        if topology.cost_per_gb:
             console.print(
-                f"  [bold][blue]Estimated egress cost:[/blue][/bold] [bright_black]${dp.topology.cost_per_gb:,.2f}/GB[/bright_black]"
+                f"  [bold][blue]Estimated egress cost:[/blue][/bold] [bright_black]${topology.cost_per_gb:,.2f}/GB[/bright_black]"
             )
         # show spinner
         with Progress(
             TextColumn(" "),
             SpinnerColumn(),
             TextColumn(f"[bright_black]Querying objects for transfer...[/bright_black]"),
             transient=True,
@@ -199,18 +238,20 @@
                 try:
                     obj_pairs.append(next(transfer_pair_gen))
                 except StopIteration:
                     break
         if len(obj_pairs) == 0:
             typer.secho("No objects to transfer.")
             return False
-        for src_obj, dst_obj in obj_pairs[:query_n]:
-            console.print(
-                f"  [bright_black][bold]{src_obj.full_path()}[/bold] => [bold]{dst_obj.full_path()}[/bold] ({format_bytes(src_obj.size)})[/bright_black]"
-            )
+        for pair in obj_pairs[:query_n]:
+            src_obj = pair.src_obj
+            for dst_obj in pair.dst_objs.values():
+                console.print(
+                    f"  [bright_black][bold]{src_obj.full_path()}[/bold] => [bold]{dst_obj.full_path()}[/bold] ({format_bytes(src_obj.size)})[/bright_black]"
+                )
         if len(obj_pairs) > query_n:
             console.print(f"  [bright_black]...[/bright_black]")
         if ask_to_confirm_transfer:
             if typer.confirm("Continue?", default=True):
                 logger.fs.debug("User confirmed transfer")
                 console.print(
                     "[green]Transfer starting[/green] (Tip: Enable auto-confirmation with `skyplane config set autoconfirm true`)"
@@ -220,46 +261,163 @@
                 logger.fs.error("Transfer cancelled by user.")
                 console.print("[bold][red]Transfer cancelled by user.[/red][/bold]")
                 raise typer.Abort()
         else:
             console.print("[green]Transfer starting[/green]")
             return True
 
-    def estimate_small_transfer(self, dp: skyplane.Dataplane, size_threshold_bytes: float, query_n: int = 1000) -> bool:
+    def estimate_small_transfer(self, job: TransferJob, size_threshold_bytes: float, query_n: int = 1000) -> bool:
         """Estimates if the transfer is small by querying up to `query_n` files from the TransferJob. If it exceeds
         the file size limit, then it will fall back to the cloud CLIs."""
-        if len(dp.jobs_to_dispatch) != 1:
-            return False
-        job = dp.jobs_to_dispatch[0]
+
+        # TODO: why shouldn't this include sync?
         if not isinstance(job, CopyJob):
             return False
         transfer_pair_gen = job.gen_transfer_pairs()
         total_size = 0
         generator_exhausted = False
         for _ in range(query_n):
             try:
-                src_obj, _ = next(transfer_pair_gen)
+                pair = next(transfer_pair_gen)
+                src_obj = pair.src_obj
                 total_size += src_obj.size
                 if total_size > size_threshold_bytes:
                     return False
             except StopIteration:
                 generator_exhausted = True
                 break
         if generator_exhausted and total_size < size_threshold_bytes:
             return True
         else:
             return False
 
 
-def force_deprovision(dp: skyplane.Dataplane, debug: bool = False):
+def force_deprovision(dp: skyplane.Dataplane):
     s = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    dp.deprovision(debug=debug)
+    dp.deprovision()
     signal.signal(signal.SIGINT, s)
 
 
+def run_transfer(
+    src: str,
+    dst: str,
+    recursive: bool,
+    debug: bool,
+    multipart: bool,
+    confirm: bool,
+    max_instances: int,
+    max_connections: int,
+    solver: str,
+    cmd: str,
+):
+    assert cmd == "cp" or cmd == "sync", f"Invalid command: {cmd}"
+    if not debug:
+        register_exception_handler()
+    print_header()
+
+    provider_src, bucket_src, path_src = parse_path(src)
+    provider_dst, bucket_dst, path_dst = parse_path(dst)
+
+    # update planner for one-sided transfer
+    # somet process for other cloud providers with no VM support
+    assert provider_src != "cloudflare" or provider_dst != "cloudflare", "Cannot transfer between two Cloudflare buckets"
+    if provider_src == "cloudflare":
+        solver = "dst_one_sided"
+    elif provider_dst == "cloudflare":
+        solver = "src_one_sided"
+
+    src_region_tag = StorageInterface.create(f"{provider_src}:infer", bucket_src).region_tag()
+    dst_region_tag = StorageInterface.create(f"{provider_dst}:infer", bucket_dst).region_tag()
+    args = {
+        "cmd": cmd,
+        "recursive": True,
+        "debug": debug,
+        "multipart": multipart,
+        "confirm": confirm,
+        "max_instances": max_instances,
+        "max_connections": max_connections,
+        "solver": solver,
+    }
+
+    # create CLI object
+    cli = SkyplaneCLI(src_region_tag=src_region_tag, dst_region_tag=dst_region_tag, args=args)
+    if not cli.check_config():
+        typer.secho(
+            f"Skyplane configuration file is not valid. Please reset your config by running `rm {config_path}` and then rerunning `skyplane init` to fix.",
+            fg="red",
+        )
+        return 1
+
+    # create pipeline and queue transfer
+    pipeline = cli.make_pipeline(planning_algorithm=solver, max_instances=max_instances)
+    if cli.args["cmd"] == "cp":
+        pipeline.queue_copy(src, dst, recursive=recursive)
+    else:
+        pipeline.queue_sync(src, dst)
+
+    # confirm transfer
+    if not cli.confirm_transfer(pipeline, src_region_tag, [dst_region_tag], 5, ask_to_confirm_transfer=not confirm):
+        return 1
+
+    # local->local transfers not supported (yet)
+    if provider_src == "local" and provider_dst == "local":
+        raise NotImplementedError("Local->local transfers not supported (yet)")
+
+    # fall back options: local->cloud, cloud->local, small cloud->cloud transfers
+    if provider_src == "local" or provider_dst == "local":
+        if cli.args["cmd"] == "cp":
+            return 0 if cli.transfer_cp_onprem(src, dst, recursive) else 1
+        else:
+            return 0 if cli.transfer_sync_onprem(src, dst) else 1
+    elif cloud_config.get_flag("native_cmd_enabled"):
+        # fallback option: transfer is too small
+        if cli.args["cmd"] == "cp":
+            job = CopyJob(src, [dst], recursive=recursive)  # TODO: rever to using pipeline
+            if cli.estimate_small_transfer(job, cloud_config.get_flag("native_cmd_threshold_gb") * GB):
+                small_transfer_status = cli.transfer_cp_small(src, dst, recursive)
+                return 0 if small_transfer_status else 1
+        else:
+            job = SyncJob(src, [dst])
+            if cli.estimate_small_transfer(job, cloud_config.get_flag("native_cmd_threshold_gb") * GB):
+                small_transfer_status = cli.transfer_sync_small(src, dst)
+                return 0 if small_transfer_status else 1
+
+    # dataplane must be created after transfers are queued
+    dp = pipeline.create_dataplane(debug=debug)
+    with dp.auto_deprovision():
+        try:
+            dp.provision(spinner=True)
+            dp.run(pipeline.jobs_to_dispatch, hooks=ProgressBarTransferHook(dp.topology.dest_region_tags))
+        except KeyboardInterrupt:
+            logger.fs.warning("Transfer cancelled by user (KeyboardInterrupt).")
+            console.print("\n[red]Transfer cancelled by user. Copying gateway logs and exiting.[/red]")
+            try:
+                dp.copy_gateway_logs()
+                force_deprovision(dp)
+            except Exception as e:
+                logger.fs.exception(e)
+                console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
+                console.print(e)
+                UsageClient.log_exception("cli_cp", e, args, cli.src_region_tag, cli.dst_region_tag)
+                console.print("[bold red]Deprovisioning was interrupted! VMs may still be running which will incur charges.[/bold red]")
+                console.print("[bold red]Please manually deprovision the VMs by running `skyplane deprovision`.[/bold red]")
+            return 1
+        except skyplane.exceptions.SkyplaneException as e:
+            console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
+            console.print(e.pretty_print_str())
+            UsageClient.log_exception("cli_query_objstore", e, args, cli.src_region_tag, cli.dst_region_tag)
+            force_deprovision(dp)
+        except Exception as e:
+            logger.fs.exception(e)
+            console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
+            console.print(e)
+            UsageClient.log_exception("cli_query_objstore", e, args, cli.src_region_tag, cli.dst_region_tag)
+            force_deprovision(dp)
+
+
 def cp(
     src: str,
     dst: str,
     recursive: bool = typer.Option(False, "--recursive", "-r", help="If true, will copy objects at folder prefix recursively"),
     debug: bool = typer.Option(False, help="If true, will write debug information to debug directory."),
     multipart: bool = typer.Option(cloud_config.get_flag("multipart_enabled"), help="If true, will use multipart uploads."),
     # transfer flags
@@ -297,93 +455,15 @@
     :param max_instances: The maximum number of instances to use per region (default: 1)
     :type max_instances: int
     :param max_connections: The maximum number of connections per instance (default: 32)
     :type max_connections: int
     :param solver: The solver to use for the transfer (default: direct)
     :type solver: str
     """
-    if not debug:
-        register_exception_handler()
-    print_header()
-    provider_src, bucket_src, path_src = parse_path(src)
-    provider_dst, bucket_dst, path_dst = parse_path(dst)
-    src_region_tag = ObjectStoreInterface.create(f"{provider_src}:infer", bucket_src).region_tag()
-    dst_region_tag = ObjectStoreInterface.create(f"{provider_dst}:infer", bucket_dst).region_tag()
-    args = {
-        "cmd": "cp",
-        "recursive": recursive,
-        "debug": debug,
-        "multipart": multipart,
-        "confirm": confirm,
-        "max_instances": max_instances,
-        "max_connections": max_connections,
-        "solver": solver,
-    }
-
-    cli = SkyplaneCLI(src_region_tag=src_region_tag, dst_region_tag=dst_region_tag, args=args)
-    if not cli.check_config():
-        typer.secho(
-            f"Skyplane configuration file is not valid. Please reset your config by running `rm {config_path}` and then rerunning `skyplane init` to fix.",
-            fg="red",
-        )
-        return 1
-
-    if provider_src in ("local", "hdfs", "nfs") or provider_dst in ("local", "hdfs", "nfs"):
-        if provider_src == "hdfs" or provider_dst == "hdfs":
-            typer.secho("HDFS is not supported yet.", fg="red")
-            return 1
-        return 0 if cli.transfer_cp_onprem(src, dst, recursive) else 1
-    elif provider_src in ("aws", "gcp", "azure") and provider_dst in ("aws", "gcp", "azure"):
-        # todo support ILP solver params
-        dp = cli.make_dataplane(
-            solver_type=solver,
-            solver_required_throughput_gbits=solver_required_throughput_gbits,
-            n_vms=max_instances,
-            n_connections=max_connections,
-        )
-        with dp.auto_deprovision():
-            dp.queue_copy(src, dst, recursive=recursive)
-            if cloud_config.get_flag("native_cmd_enabled") and cli.estimate_small_transfer(
-                dp, cloud_config.get_flag("native_cmd_threshold_gb") * GB
-            ):
-                small_transfer_status = cli.transfer_cp_small(src, dst, recursive)
-                if small_transfer_status:
-                    return 0
-            try:
-                if not cli.confirm_transfer(dp, 5, ask_to_confirm_transfer=not confirm):
-                    return 1
-                dp.provision(spinner=True)
-                dp.run(ProgressBarTransferHook())
-            except KeyboardInterrupt:
-                logger.fs.warning("Transfer cancelled by user (KeyboardInterrupt).")
-                console.print("\n[red]Transfer cancelled by user. Copying gateway logs and exiting.[/red]")
-                do_parallel(dp.copy_log, dp.bound_nodes.values(), n=-1)
-                try:
-                    force_deprovision(dp, debug=debug)
-                except Exception as e:
-                    logger.fs.exception(e)
-                    console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
-                    console.print(e)
-                    UsageClient.log_exception("cli_cp", e, args, cli.src_region_tag, cli.dst_region_tag)
-                    console.print("[bold red]Deprovisioning was interrupted! VMs may still be running which will incur charges.[/bold red]")
-                    console.print("[bold red]Please manually deprovision the VMs by running `skyplane deprovision`.[/bold red]")
-                return 1
-            except skyplane.exceptions.SkyplaneException as e:
-                console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
-                console.print(e.pretty_print_str())
-                UsageClient.log_exception("cli_query_objstore", e, args, cli.src_region_tag, cli.dst_region_tag)
-                force_deprovision(dp, debug=debug)
-            except Exception as e:
-                logger.fs.exception(e)
-                console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
-                console.print(e)
-                UsageClient.log_exception("cli_query_objstore", e, args, cli.src_region_tag, cli.dst_region_tag)
-                force_deprovision(dp, debug=debug)
-        if dp.provisioned:
-            typer.secho("Dataplane is not deprovisioned! Run `skyplane deprovision` to force deprovision VMs.", fg="red")
+    return run_transfer(src, dst, recursive, debug, multipart, confirm, max_instances, max_connections, solver, "cp")
 
 
 def sync(
     src: str,
     dst: str,
     debug: bool = typer.Option(False, help="If true, will write debug information to debug directory."),
     multipart: bool = typer.Option(cloud_config.get_flag("multipart_enabled"), help="If true, will use multipart uploads."),
@@ -424,88 +504,8 @@
     :param max_instances: The maximum number of instances to use per region (default: 1)
     :type max_instances: int
     :param max_connections: The maximum number of connections per instance (default: 32)
     :type max_connections: int
     :param solver: The solver to use for the transfer (default: direct)
     :type solver: str
     """
-    if not debug:
-        register_exception_handler()
-    print_header()
-    provider_src, bucket_src, path_src = parse_path(src)
-    provider_dst, bucket_dst, path_dst = parse_path(dst)
-    src_region_tag = ObjectStoreInterface.create(f"{provider_src}:infer", bucket_src).region_tag()
-    dst_region_tag = ObjectStoreInterface.create(f"{provider_dst}:infer", bucket_dst).region_tag()
-    args = {
-        "cmd": "sync",
-        "recursive": True,
-        "debug": debug,
-        "multipart": multipart,
-        "confirm": confirm,
-        "max_instances": max_instances,
-        "max_connections": max_connections,
-        "solver": solver,
-    }
-
-    cli = SkyplaneCLI(src_region_tag=src_region_tag, dst_region_tag=dst_region_tag, args=args)
-    if not cli.check_config():
-        typer.secho(
-            f"Skyplane configuration file is not valid. Please reset your config by running `rm {config_path}` and then rerunning `skyplane init` to fix.",
-            fg="red",
-        )
-        return 1
-
-    if provider_src in ("local", "hdfs", "nfs") or provider_dst in ("local", "hdfs", "nfs"):
-        if provider_src == "hdfs" or provider_dst == "hdfs":
-            typer.secho("HDFS is not supported yet.", fg="red")
-            return 1
-        return 0 if cli.transfer_sync_onprem(src, dst) else 1
-    elif provider_src in ("aws", "gcp", "azure") and provider_dst in ("aws", "gcp", "azure"):
-        # todo support ILP solver params
-        print()
-        dp = cli.make_dataplane(
-            solver_type=solver,
-            solver_required_throughput_gbits=solver_required_throughput_gbits,
-            n_vms=max_instances,
-            n_connections=max_connections,
-        )
-        with dp.auto_deprovision():
-            dp.queue_sync(src, dst)
-            if cloud_config.get_flag("native_cmd_enabled") and cli.estimate_small_transfer(
-                dp, cloud_config.get_flag("native_cmd_threshold_gb") * GB
-            ):
-                small_transfer_status = cli.transfer_sync_small(src, dst)
-                if small_transfer_status:
-                    return 0
-            try:
-                console.print("[yellow]Note: sync must query the destination bucket to diff objects. This may take a while.[/yellow]")
-                if not cli.confirm_transfer(dp, 5, ask_to_confirm_transfer=not confirm):
-                    return 1
-                dp.provision(spinner=True)
-                dp.run(ProgressBarTransferHook())
-            except KeyboardInterrupt:
-                logger.fs.warning("Transfer cancelled by user (KeyboardInterrupt).")
-                console.print("\n[red]Transfer cancelled by user. Copying gateway logs and exiting.[/red]")
-                do_parallel(dp.copy_log, dp.bound_nodes.values(), n=-1)
-                try:
-                    force_deprovision(dp, debug=debug)
-                except Exception as e:
-                    logger.fs.exception(e)
-                    console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
-                    console.print(e)
-                    UsageClient.log_exception("cli_cp", e, args, cli.src_region_tag, cli.dst_region_tag)
-                    console.print("[bold red]Deprovisioning was interrupted! VMs may still be running which will incur charges.[/bold red]")
-                    console.print("[bold red]Please manually deprovision the VMs by running `skyplane deprovision`.[/bold red]")
-                return 1
-            except skyplane.exceptions.SkyplaneException as e:
-                console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
-                console.print(e.pretty_print_str())
-                UsageClient.log_exception("cli_query_objstore", e, args, cli.src_region_tag, cli.dst_region_tag)
-                return 1
-            except Exception as e:
-                logger.fs.exception(e)
-                console.print(f"[bright_black]{traceback.format_exc()}[/bright_black]")
-                console.print(e)
-                UsageClient.log_exception("cli_query_objstore", e, args, cli.src_region_tag, cli.dst_region_tag)
-                force_deprovision(dp, debug=debug)
-        if dp.provisioned:
-            typer.secho("Dataplane is not deprovisioned! Run `skyplane deprovision` to force deprovision VMs.", fg="red")
+    return run_transfer(src, dst, False, debug, multipart, confirm, max_instances, max_connections, solver, "sync")
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/cli_profile.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/cli_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
 import random
 import sys
 from datetime import datetime, timezone
 from pathlib import Path
 
-import pandas as pd
 import typer
 from rich.progress import Progress
 from typing import List, Optional, Tuple
 
 from skyplane import __root__
 from skyplane import compute
 from skyplane.cli.experiments.provision import provision
@@ -18,14 +17,15 @@
 from skyplane.utils.definitions import GB
 from skyplane.utils.fn import do_parallel
 
 all_aws_regions = compute.AWSCloudProvider.region_list()
 all_azure_regions = compute.AzureCloudProvider.region_list()
 all_gcp_regions = compute.GCPCloudProvider.region_list()
 all_gcp_regions_standard = compute.GCPCloudProvider.region_list_standard()
+all_ibmcloud_regions = compute.IBMCloudProvider.region_list()
 
 
 def split_list(l):
     pairs = set(l)
     groups = []
     elems_in_last_group = set()
     while pairs:
@@ -91,26 +91,31 @@
     ),
     copy_resume_file: bool = typer.Option(True, help="Copy the resume file to the output CSV. Default is True."),
     # regions
     aws_region_list: List[str] = typer.Option(all_aws_regions, "-aws"),
     azure_region_list: List[str] = typer.Option(all_azure_regions, "-azure"),
     gcp_region_list: List[str] = typer.Option(all_gcp_regions, "-gcp"),
     gcp_standard_region_list: List[str] = typer.Option(all_gcp_regions_standard, "-gcp-standard"),
+    ibmcloud_region_list: List[str] = typer.Option(all_ibmcloud_regions, "-ibmcloud"),
     enable_aws: bool = typer.Option(True),
     enable_azure: bool = typer.Option(True),
     enable_gcp: bool = typer.Option(True),
     enable_gcp_standard: bool = typer.Option(True),
+    enable_ibmcloud: bool = typer.Option(True),
     # instances to provision
     aws_instance_class: str = typer.Option("m5.8xlarge", help="AWS instance class to use"),
     azure_instance_class: str = typer.Option("Standard_D32_v5", help="Azure instance class to use"),
     gcp_instance_class: str = typer.Option("n2-standard-32", help="GCP instance class to use"),
+    ibmcloud_instance_class: str = typer.Option("bx2-2x8", help="IBM Cloud instance class to use"),
     # iperf3 options
     iperf3_runtime: int = typer.Option(5, help="Runtime for iperf3 in seconds"),
     iperf3_connections: int = typer.Option(64, help="Number of connections to test"),
 ):
+    import pandas as pd
+
     def check_stderr(tup):
         assert tup[1].strip() == "", f"Command failed, err: {tup[1]}"
 
     if resume:
         index_key = [
             "iperf3_connections",
             "iperf3_runtime",
@@ -126,16 +131,17 @@
     else:
         resume_keys = []
 
     # validate arguments
     aws_region_list = aws_region_list if enable_aws else []
     azure_region_list = azure_region_list if enable_azure else []
     gcp_region_list = gcp_region_list if enable_gcp else []
-    if not enable_aws and not enable_azure and not enable_gcp:
-        logger.error("At least one of -aws, -azure, -gcp must be enabled.")
+    ibmcloud_region_list = ibmcloud_region_list if enable_ibmcloud else []
+    if not enable_aws and not enable_azure and not enable_gcp and not enable_ibmcloud:
+        logger.error("At least one of -aws, -azure, -gcp, -ibmcloud must be enabled.")
         raise typer.Abort()
 
     # validate AWS regions
     if not enable_aws:
         aws_region_list = []
     elif not all(r in all_aws_regions for r in aws_region_list):
         logger.error(f"Invalid AWS region list: {aws_region_list}")
@@ -159,47 +165,62 @@
     # validate GCP standard instances
     if not enable_gcp_standard:
         gcp_standard_region_list = []
     if not all(r in all_gcp_regions_standard for r in gcp_standard_region_list):
         logger.error(f"Invalid GCP standard region list: {gcp_standard_region_list}")
         raise typer.Abort()
 
+    # validate IBM Cloud regions
+    if not enable_ibmcloud:
+        ibmcloud_region_list = []
+    elif not all(r in all_ibmcloud_regions for r in ibmcloud_region_list):
+        logger.error(f"Invalid IBM Cloud region list: {ibmcloud_region_list}")
+        raise typer.Abort()
+
     # provision servers
     aws = compute.AWSCloudProvider()
     azure = compute.AzureCloudProvider()
     gcp = compute.GCPCloudProvider()
-    aws_instances, azure_instances, gcp_instances = provision(
+    ibmcloud = compute.IBMCloudProvider()
+
+    aws_instances, azure_instances, gcp_instances, ibmcloud_instances = provision(
         aws=aws,
         azure=azure,
         gcp=gcp,
+        ibmcloud=ibmcloud,
         aws_regions_to_provision=aws_region_list,
         azure_regions_to_provision=azure_region_list,
         gcp_regions_to_provision=gcp_region_list,
+        ibmcloud_regions_to_provision=ibmcloud_region_list,
         aws_instance_class=aws_instance_class,
         azure_instance_class=azure_instance_class,
         gcp_instance_class=gcp_instance_class,
+        ibmcloud_instance_class=ibmcloud_instance_class,
         aws_instance_os="ubuntu",
         gcp_instance_os="ubuntu",
         gcp_use_premium_network=True,
     )
     instance_list: List[compute.Server] = [i for ilist in aws_instances.values() for i in ilist]
     instance_list.extend([i for ilist in azure_instances.values() for i in ilist])
     instance_list.extend([i for ilist in gcp_instances.values() for i in ilist])
 
     # provision standard tier servers
-    _, _, gcp_standard_instances = provision(
+    _, _, gcp_standard_instances, _ = provision(
         aws=aws,
         azure=azure,
         gcp=gcp,
+        ibmcloud=ibmcloud,
         aws_regions_to_provision=[],
         azure_regions_to_provision=[],
+        ibmcloud_regions_to_provision=[],
         gcp_regions_to_provision=gcp_standard_region_list,
         aws_instance_class=aws_instance_class,
         azure_instance_class=azure_instance_class,
         gcp_instance_class=gcp_instance_class,
+        ibmcloud_instance_class=ibmcloud_instance_class,
         aws_instance_os="ubuntu",
         gcp_instance_os="ubuntu",
         gcp_use_premium_network=False,
     )
     instance_list.extend([i for ilist in gcp_standard_instances.values() for i in ilist])
 
     # setup instances
@@ -323,34 +344,40 @@
 
 
 def latency_grid(
     aws_region_list: List[str] = typer.Option(all_aws_regions, "-aws"),
     azure_region_list: List[str] = typer.Option(all_azure_regions, "-azure"),
     gcp_region_list: List[str] = typer.Option(all_gcp_regions, "-gcp"),
     gcp_standard_region_list: List[str] = typer.Option(all_gcp_regions_standard, "-gcp-standard"),
+    ibmcloud_region_list: List[str] = typer.Option(all_ibmcloud_regions, "-gcp"),
     enable_aws: bool = typer.Option(True),
     enable_azure: bool = typer.Option(True),
     enable_gcp: bool = typer.Option(True),
     enable_gcp_standard: bool = typer.Option(True),
+    enable_ibmcloud: bool = typer.Option(True),
     # instances to provision
     aws_instance_class: str = typer.Option("m5.large", help="AWS instance class to use"),
     azure_instance_class: str = typer.Option("Standard_D2_v3", help="Azure instance class to use"),
     gcp_instance_class: str = typer.Option("n2-standard-4", help="GCP instance class to use"),
+    ibmcloud_instance_class: str = typer.Option("bx2-2x8", help="IBM Cloud instance class to use"),
 ):
+    import pandas as pd
+
     # similar to throughput_grid but start all instances at once and then ping all pairs of instances concurrently
 
     def check_stderr(tup):
         assert tup[1].strip() == "", f"Command failed, err: {tup[1]}"
 
     # validate arguments
     aws_region_list = aws_region_list if enable_aws else []
     azure_region_list = azure_region_list if enable_azure else []
     gcp_region_list = gcp_region_list if enable_gcp else []
-    if not enable_aws and not enable_azure and not enable_gcp:
-        logger.error("At least one of -aws, -azure, -gcp must be enabled.")
+    ibmcloud_region_list = ibmcloud_region_list if enable_ibmcloud else []
+    if not enable_aws and not enable_azure and not enable_gcp and not enable_ibmcloud:
+        logger.error("At least one of -aws, -azure, -gcp, -ibmcloud must be enabled.")
         raise typer.Abort()
 
     # validate AWS regions
     if not enable_aws:
         aws_region_list = []
     elif not all(r in all_aws_regions for r in aws_region_list):
         logger.error(f"Invalid AWS region list: {aws_region_list}")
@@ -376,45 +403,60 @@
     # validate GCP standard instances
     if not enable_gcp_standard:
         gcp_standard_region_list = []
     if not all(r in all_gcp_regions_standard for r in gcp_standard_region_list):
         logger.error(f"Invalid GCP standard region list: {gcp_standard_region_list}")
         raise typer.Abort()
 
+    # validate IBM Cloud regions
+    if not enable_ibmcloud:
+        ibmcloud_region_list = []
+    elif not all(r in all_ibmcloud_regions for r in ibmcloud_region_list):
+        logger.error(f"Invalid IBM Cloud region list: {ibmcloud_region_list}")
+        raise typer.Abort()
+
     # provision servers
     aws = compute.AWSCloudProvider()
     azure = compute.AzureCloudProvider()
     gcp = compute.GCPCloudProvider()
-    aws_instances, azure_instances, gcp_instances = provision(
+    ibmcloud = compute.IBMCloudProvider()
+    aws_instances, azure_instances, gcp_instances, ibmcloud_instances = provision(
         aws=aws,
         azure=azure,
         gcp=gcp,
+        ibmcloud=ibmcloud,
         aws_regions_to_provision=aws_region_list,
         azure_regions_to_provision=azure_region_list,
         gcp_regions_to_provision=gcp_region_list,
+        ibmcloud_regions_to_provision=ibmcloud_region_list,
         aws_instance_class=aws_instance_class,
         azure_instance_class=azure_instance_class,
         gcp_instance_class=gcp_instance_class,
+        ibmcloud_instance_class=ibmcloud_instance_class,
         gcp_use_premium_network=True,
     )
     instance_list: List[compute.Server] = [i for ilist in aws_instances.values() for i in ilist]
     instance_list.extend([i for ilist in azure_instances.values() for i in ilist])
     instance_list.extend([i for ilist in gcp_instances.values() for i in ilist])
+    instance_list.extend([i for ilist in ibmcloud_instances.values() for i in ilist])
 
     # provision standard tier servers
-    _, _, gcp_standard_instances = provision(
+    _, _, gcp_standard_instances, _ = provision(
         aws=aws,
         azure=azure,
         gcp=gcp,
+        ibmcloud=ibmcloud,
         aws_regions_to_provision=[],
         azure_regions_to_provision=[],
         gcp_regions_to_provision=gcp_standard_region_list,
+        ibmcloud_regions_to_provision=[],
         aws_instance_class=aws_instance_class,
         azure_instance_class=azure_instance_class,
         gcp_instance_class=gcp_instance_class,
+        ibmcloud_instance_class=ibmcloud_instance_class,
         gcp_use_premium_network=False,
     )
     instance_list.extend([i for ilist in gcp_standard_instances.values() for i in ilist])
 
     # setup instances
     def setup(server: compute.Server):
         check_stderr(server.run_command(make_sysctl_tcp_tuning_command(cc="cubic")))
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/cli_query.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/cli_query.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/experiments/provision.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/experiments/provision.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,43 +23,56 @@
     return {r: ilist for r, ilist in results if ilist}
 
 
 def provision(
     aws: compute.AWSCloudProvider,
     azure: compute.AzureCloudProvider,
     gcp: compute.GCPCloudProvider,
+    ibmcloud: compute.IBMCloudProvider,
     aws_regions_to_provision: List[str],
     azure_regions_to_provision: List[str],
     gcp_regions_to_provision: List[str],
+    ibmcloud_regions_to_provision: List[str],
     aws_instance_class: str,
     azure_instance_class: str,
     gcp_instance_class: str,
+    ibmcloud_instance_class: str,
     aws_instance_os: str = "ecs-aws-linux-2",
     gcp_instance_os: str = "cos",
     azure_instance_os: str = "ubuntu",
     gcp_use_premium_network: bool = True,
     log_dir: Optional[str] = None,
-) -> Tuple[Dict[str, List[compute.AWSServer]], Dict[str, List[compute.AzureServer]], Dict[str, List[compute.GCPServer]]]:
+) -> Tuple[
+    Dict[str, List[compute.AWSServer]],
+    Dict[str, List[compute.AzureServer]],
+    Dict[str, List[compute.GCPServer]],
+    Dict[str, List[compute.IBMCloudServer]],
+]:
     """Provision list of instances in AWS, Azure, and GCP in each specified region."""
     aws_instances = {}
     azure_instances = {}
     gcp_instances = {}
+    ibmcloud_instances = {}
 
     # TODO: It might be significantly faster to provision AWS, Azure, and GCP concurrently (e.g., using threads)
 
     jobs = []
     jobs.append(partial(aws.setup_global, attach_policy_arn="arn:aws:iam::aws:policy/AmazonS3FullAccess"))
     if aws_regions_to_provision:
         for r in set(aws_regions_to_provision):
             jobs.append(partial(aws.setup_region, r))
     if azure_regions_to_provision:
         jobs.append(azure.create_ssh_key)
         jobs.append(azure.set_up_resource_group)
     if gcp_regions_to_provision:
         jobs.append(gcp.setup_global)
+    if ibmcloud_regions_to_provision:
+        for r in set(ibmcloud_regions_to_provision):
+            jobs.append(partial(ibmcloud.setup_region, r.split(":")[1]))
+
     with Timer("Cloud SSH key initialization"):
         do_parallel(lambda fn: fn(), jobs)
 
     if len(aws_regions_to_provision) > 0:
         logger.info(f"Provisioning AWS instances in {aws_regions_to_provision}")
         aws_instance_filter = {
             "tags": {"skyplane": "true"},
@@ -141,18 +154,37 @@
             results = do_parallel(
                 gcp_provisioner, missing_gcp_regions, spinner=True, desc=f"provision GCP (premium network = {gcp_use_premium_network})"
             )
             for region, result in results:
                 gcp_instances[region] = [result]
             gcp_instances = refresh_instance_list(gcp, gcp_regions_to_provision, gcp_instance_filter)
 
+    if len(ibmcloud_regions_to_provision) > 0:
+        logger.info(f"Provisioning IBM Cloud instances in {ibmcloud_regions_to_provision}")
+        ibmcloud_instance_filter = {
+            "tags": {"skyplane": "true"},
+            "instance_type": ibmcloud_instance_class,
+            "state": [compute.ServerState.PENDING, compute.ServerState.RUNNING],
+        }
+        do_parallel(aws.add_ips_to_security_group, ibmcloud_regions_to_provision, spinner=True, desc="Add IP to IBM Cloud security groups")
+        ibmcloud_instances = refresh_instance_list(ibmcloud, ibmcloud_regions_to_provision, ibmcloud_instance_filter)
+        missing_ibmcloud_regions = set(ibmcloud_regions_to_provision) - set(ibmcloud_instances.keys())
+        if missing_ibmcloud_regions:
+            logger.info(f"(IBM Cloud) provisioning missing regions: {missing_ibmcloud_regions}")
+            ibmcloud_provisioner = lambda r: ibmcloud.provision_instance(r, ibmcloud_instance_class)
+            results = do_parallel(ibmcloud_provisioner, missing_ibmcloud_regions, spinner=True, desc="provision IBM Cloud")
+            for region, result in results:
+                aws_instances[region] = [result]
+            aws_instances = refresh_instance_list(ibmcloud, ibmcloud_regions_to_provision, ibmcloud_instance_filter)
+
     # init log files
     def init(i: compute.Server):
         i.init_log_files(log_dir)
 
     all_instances = (
         [i for ilist in aws_instances.values() for i in ilist]
         + [i for ilist in azure_instances.values() for i in ilist]
         + [i for ilist in gcp_instances.values() for i in ilist]
+        + [i for ilist in ibmcloud_instances.values() for i in ilist]
     )
     do_parallel(init, all_instances, spinner=True, desc="Provisioning init")
-    return aws_instances, azure_instances, gcp_instances  # pytype: disable=bad-return-type
+    return aws_instances, azure_instances, gcp_instances, ibmcloud_instances  # pytype: disable=bad-return-type
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/impl/common.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/impl/common.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/cli/impl/cp_replicate_fallback.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/cli/impl/cp_replicate_fallback.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/__init__.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from skyplane.compute.aws.aws_auth import AWSAuthentication
 from skyplane.compute.aws.aws_cloud_provider import AWSCloudProvider
 from skyplane.compute.aws.aws_server import AWSServer
+from skyplane.compute.ibmcloud.ibmcloud_server import IBMCloudServer
 from skyplane.compute.azure.azure_auth import AzureAuthentication
 from skyplane.compute.azure.azure_cloud_provider import AzureCloudProvider
 from skyplane.compute.azure.azure_server import AzureServer
 from skyplane.compute.cloud_provider import CloudProvider
 from skyplane.compute.gcp.gcp_auth import GCPAuthentication
 from skyplane.compute.gcp.gcp_cloud_provider import GCPCloudProvider
 from skyplane.compute.gcp.gcp_server import GCPServer
+from skyplane.compute.ibmcloud.ibmcloud_auth import IBMCloudAuthentication
+from skyplane.compute.ibmcloud.ibmcloud_provider import IBMCloudProvider
 from skyplane.compute.server import Server, ServerState
 
 __all__ = [
     "CloudProvider",
     "Server",
     "ServerState",
     "AWSAuthentication",
     "AWSCloudProvider",
     "AWSServer",
+    "IBMCloudServer",
     "AzureAuthentication",
     "AzureCloudProvider",
     "AzureServer",
     "GCPAuthentication",
     "GCPCloudProvider",
+    "IBMCloudAuthentication",
+    "IBMCloudProvider",
     "GCPServer",
 ]
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_auth.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Optional
+from typing import Optional, Dict
+import json
 
 from skyplane.config import SkyplaneConfig
-from skyplane.config_paths import config_path, aws_config_path
-from skyplane.utils import imports
+from skyplane.config_paths import config_path, aws_config_path, aws_quota_path
+from skyplane.utils import imports, fn, logger
 
 
 class AWSAuthentication:
     def __init__(self, config: Optional[SkyplaneConfig] = None, access_key: Optional[str] = None, secret_key: Optional[str] = None):
         """Loads AWS authentication details. If no access key is provided, it will try to load credentials using boto3"""
         if not config is None:
             self.config = config
@@ -18,43 +19,75 @@
             self._access_key = access_key
             self._secret_key = secret_key
         else:
             self.config_mode = "iam_inferred"
             self._access_key = None
             self._secret_key = None
 
+    def _get_ec2_vm_quota(self, region) -> Dict[str, int]:
+        """Given the region, get the maximum number of vCPU that can be launched.
+
+        Returns:
+            name_to_quota: a dictionary of quota name to quota value
+        """
+        # NOTE: the QuotaCode can be retried via
+        # aws service-quotas list-service-quotas --service-code ec2
+        # The items we are looking is
+        # "Running On-Demand Standard (A, C, D, H, I, M, R, T, Z) instances" L-1216C47A
+        # "All Standard (A, C, D, H, I, M, R, T, Z) Spot Instance Requests" L-34B43A08
+        quotas_client = self.get_boto3_client("service-quotas", region)
+
+        name_to_quota = {}
+        for name, code in [("on_demand_standard_vcpus", "L-1216C47A"), ("spot_standard_vcpus", "L-34B43A08")]:
+            try:
+                retrieved_quota = quotas_client.get_service_quota(ServiceCode="ec2", QuotaCode=code)
+                name_to_quota[name] = int(retrieved_quota["Quota"]["Value"])
+            except Exception:
+                logger.warning(
+                    f"Failed to retrieve quota information for {name} in {region}. Skyplane will use a conservative configuration."
+                )
+        return name_to_quota
+
     @imports.inject("boto3", pip_extra="aws")
     def save_region_config(boto3, self, config: SkyplaneConfig):
         if not config.aws_enabled:
             self.clear_region_config()
             return
         with aws_config_path.open("w") as f:
             region_list = []
+
+            # query regions
             describe_regions = boto3.client("ec2", region_name="us-east-1").describe_regions()
             for region in describe_regions["Regions"]:
                 if region["OptInStatus"] == "opt-in-not-required" or region["OptInStatus"] == "opted-in":
                     region_text = region["Endpoint"]
                     region_name = region_text[region_text.find(".") + 1 : region_text.find(".amazon")]
                     region_list.append(region_name)
             f.write("\n".join(region_list))
 
+        quota_infos = fn.do_parallel(
+            self._get_ec2_vm_quota, region_list, return_args=False, spinner=True, desc="Retrieving EC2 Quota information"
+        )
+        region_infos = [dict(**info, **{"region_name": name}) for name, info in zip(region_list, quota_infos)]
+        with aws_quota_path.open("w") as f:
+            f.write(json.dumps(region_infos, indent=2))
+
     def clear_region_config(self):
         with aws_config_path.open("w") as f:
             f.write("")
 
     @staticmethod
     def get_region_config():
-        try:
-            f = open(aws_config_path, "r")
-        except FileNotFoundError:
+        if not aws_config_path.exists():
             return []
-        region_list = []
-        for region in f.read().split("\n"):
-            region_list.append(region)
-        return region_list
+        with aws_config_path.open() as f:
+            region_list = []
+            for region in f.read().split("\n"):
+                region_list.append(region)
+            return region_list
 
     @property
     def access_key(self):
         if self._access_key is None:
             self._access_key, self._secret_key = self.infer_credentials()
         return self._access_key
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_cloud_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,19 +224,22 @@
                     instance = start_instance(subnets[current_subnet_id].id)
                     break
                 except exceptions.ClientError as e:
                     if i == max_retries - 1:
                         raise
                     elif "VcpuLimitExceeded" in str(e):
                         raise skyplane_exceptions.InsufficientVCPUException() from e
-                    elif "Invalid IAM Instance Profile name" not in str(e):
+                    elif "Invalid IAM Instance Profile name" in str(e):
+                        # TODO: suppress this
                         logger.warning(str(e))
                     elif "InsufficientInstanceCapacity" in str(e):
                         # try another subnet
                         current_subnet_id = (current_subnet_id + 1) % len(subnets)
+                    else:
+                        raise ValueError(f"Unexpected provisioning error: {str(e)}")
                     time.sleep(backoff)
                     backoff = min(backoff * 2, max_backoff)
 
             assert len(instance) == 1, f"Expected 1 instance, got {len(instance)}"
             try:
                 instance[0].wait_until_running()
             except KeyboardInterrupt:
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_key_manager.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_network.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_network.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_pricing.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_pricing.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/aws/aws_server.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/aws/aws_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,15 @@
 
         sshtunnel.DEFAULT_LOGLEVEL = logging.FATAL
         return sshtunnel.SSHTunnelForwarder(
             (self.public_ip(), 22),
             # ssh_username="ec2-user",
             ssh_username=self.login_name,
             ssh_pkey=str(self.local_keyfile),
+            host_pkey_directories=[],
             local_bind_address=("127.0.0.1", 0),
             remote_bind_address=("127.0.0.1", remote_port),
         )
 
     def get_ssh_cmd(self):
         # return f"ssh -i {self.local_keyfile} ec2-user@{self.public_ip()}"
         return f"ssh -i {self.local_keyfile} {self.login_name}@{self.public_ip()}"
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/azure/azure_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/azure/azure_cloud_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         return AzureAuthentication.get_region_config()
 
     @staticmethod
     def lookup_continent(region: str) -> str:
         lookup_dict = {
             "oceania": {"australiaeast", "australiacentral", "australiasoutheast", "australiacentral2"},
             "asia": {
+                "qatarcentral",
                 "eastasia",
                 "japaneast",
                 "japanwest",
                 "koreacentral",
                 "koreasouth",
                 "southeastasia",
                 "southindia",
@@ -216,15 +217,15 @@
         if resource_client.resource_groups.check_existence(AzureServer.resource_group_name):
             # Resource group already exists.
             # Take this moment to search for orphaned resources and clean them up...
             network_client = self.auth.get_network_client()
             if clean_up_orphans:
                 instances_to_terminate = []
                 for vnet in network_client.virtual_networks.list(AzureServer.resource_group_name):
-                    if vnet.tags.get("skyplane", None) == "true" and AzureServer.is_valid_vnet_name(vnet.name):
+                    if vnet.tags and vnet.tags.get("skyplane", None) == "true" and AzureServer.is_valid_vnet_name(vnet.name):
                         name = AzureServer.base_name_from_vnet_name(vnet.name)
                         s = AzureServer(name, assume_exists=False)
                         if not s.is_valid():
                             instances_to_terminate.append(s)
 
                 if len(instances_to_terminate) > 0:
                     logger.warning(
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/azure/azure_server.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/azure/azure_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,17 @@
         public_ip = network_client.public_ip_addresses.get(AzureServer.resource_group_name, AzureServer.ip_name(self.name))
 
         # Sanity checks
         assert public_ip.location == self.location
         assert public_ip.name == AzureServer.ip_name(self.name)
         return public_ip.ip_address
 
+    def private_ip(self):
+        return None
+
     @ignore_lru_cache()
     def instance_class(self):
         vm = self.get_virtual_machine()
         return vm.hardware_profile.vm_size
 
     def region(self):
         return self.location
@@ -194,13 +197,14 @@
         import sshtunnel
 
         return sshtunnel.SSHTunnelForwarder(
             (self.public_ip(), 22),
             ssh_username=uname,
             ssh_pkey=str(self.ssh_private_key),
             ssh_private_key_password=ssh_key_password,
+            host_pkey_directories=[],
             local_bind_address=("127.0.0.1", 0),
             remote_bind_address=("127.0.0.1", remote_port),
         )
 
     def get_ssh_cmd(self, uname="skyplane", ssh_key_password="skyplane"):
         return f"ssh -i {self.ssh_private_key} {uname}@{self.public_ip()}"
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/cloud_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import functools
 
 from typing import List, Optional, Union
 
 from skyplane.compute.server import Server, ServerState
 from skyplane.utils.fn import do_parallel
+from skyplane.utils import logger
 
 
 class CloudProvider:
     logging_enabled = True  # For Dozzle
     log_viewer_port = 8888
 
     @property
@@ -17,31 +18,40 @@
     @staticmethod
     def region_list():
         raise NotImplementedError
 
     @staticmethod
     @functools.lru_cache(maxsize=None)
     def get_transfer_cost(src_key, dst_key, premium_tier=True):
-        if src_key == dst_key:
-            return 0.0
         src_provider, _ = src_key.split(":")
+        if src_key == dst_key or src_provider == "cos":
+            return 0.0
+        elif src_provider == "cloudflare":
+            return 0.0  # TODO: fix this for other clouds
         if src_provider == "aws":
             from skyplane.compute.aws.aws_cloud_provider import AWSCloudProvider
 
             return AWSCloudProvider.get_transfer_cost(src_key, dst_key, premium_tier)
         elif src_provider == "gcp":
             from skyplane.compute.gcp.gcp_cloud_provider import GCPCloudProvider
 
             return GCPCloudProvider.get_transfer_cost(src_key, dst_key, premium_tier)
         elif src_provider == "azure":
             from skyplane.compute.azure.azure_cloud_provider import AzureCloudProvider
 
             return AzureCloudProvider.get_transfer_cost(src_key, dst_key, premium_tier)
+        elif src_provider == "ibmcloud":
+            logger.warning("IBM cloud costs are not yet supported.")
+            return 0
+        elif src_provider == "hdfs":
+            from skyplane.compute.gcp.gcp_cloud_provider import GCPCloudProvider
+
+            return GCPCloudProvider.get_transfer_cost(f"gcp:{_}", dst_key, premium_tier)
         else:
-            raise NotImplementedError
+            raise ValueError(f"Unknown provider {src_provider}")
 
     def get_instance_list(self, region) -> List[Server]:
         raise NotImplementedError
 
     def get_matching_instances(
         self,
         region: Optional[str] = None,
@@ -73,15 +83,15 @@
         self,
         region: str,
         instance_class: str,
         disk_size: int = 32,
         use_spot_instances: bool = False,
         name: Optional[str] = None,
         tags={"skyplane": "true"},
-        **kwargs
+        **kwargs,
     ) -> Server:
         raise NotImplementedError
 
     def setup_global(self, **kwargs):
         pass
 
     def setup_region(self, region: str):
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/const_cmds.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/const_cmds.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_auth.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import base64
 import os
 import time
+import json
 from pathlib import Path
 
 from typing import Optional
 
 from skyplane.compute.server import key_root
 from skyplane.config import SkyplaneConfig
-from skyplane.config_paths import config_path, gcp_config_path
+from skyplane.config_paths import config_path, gcp_config_path, gcp_quota_path
 from skyplane.utils import logger, imports
 from skyplane.utils.retry import retry_backoff
 
 
 class GCPAuthentication:
     def __init__(self, config: Optional[SkyplaneConfig] = None):
         if not config == None:
@@ -42,26 +43,45 @@
                     region_list.append(region["description"])
 
                 request = service.regions().list_next(previous_request=request, previous_response=response)
 
             f.write("\n".join(region_list))
             print(f"    GCP region config file saved to {gcp_config_path}")
 
+        try:
+            with gcp_quota_path.open("w") as f:
+                service = discovery.build("compute", "beta", credentials=self.credentials)
+                request = service.regions().list(project=self.project_id)
+                region_to_vcpus = {}
+                while request is not None:
+                    response = request.execute()
+                    for region in response["items"]:
+                        if region["kind"] != "compute#region":
+                            continue
+                        region_name = region["name"]
+                        for quota_item in region["quotas"]:
+                            if quota_item["metric"] == "N2_CPUS":  # Initially only concerned with N2 limits
+                                region_to_vcpus[region_name] = quota_item["limit"]
+                                break
+                    request = service.regions().list_next(previous_request=request, previous_response=response)
+                json.dump(region_to_vcpus, f)
+        except Exception:
+            logger.warning("Failed to retrieve GCP quota information. Skyplane will a conservative configuration.")
+
     @staticmethod
     def clear_region_config():
         with gcp_config_path.open("w") as f:
             f.write("")
 
     @staticmethod
     def get_region_config():
-        try:
-            f = open(gcp_config_path, "r")
-        except FileNotFoundError:
+        if not gcp_config_path.exists():
             return []
-        return [r for r in map(str.strip, f.readlines()) if r]
+        with gcp_config_path.open("r") as f:
+            return [r for r in map(str.strip, f.readlines()) if r]
 
     @property
     def credentials(self):
         if self._credentials is None:
             self._credentials, _ = self.get_adc_credential(self.project_id)
         return self._credentials
 
@@ -230,12 +250,13 @@
 
     @imports.inject("googleapiclient.discovery", pip_extra="gcp")
     def get_gcp_client(discovery, self, service_name="compute", version="v1"):
         return discovery.build(service_name, version, credentials=self.credentials, client_options={"quota_project_id": self.project_id})
 
     @imports.inject("google.cloud.storage", pip_extra="gcp")
     def get_storage_client(storage, self):
-        # must use service account for XML storage API
+        # TODO: cache storage account clinet
+        # check that storage account works
         return storage.Client.from_service_account_json(self.service_account_credentials)
 
     def get_gcp_instances(self, gcp_region: str):
         return self.get_gcp_client().instances().list(project=self.project_id, zone=gcp_region).execute()
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_cloud_provider.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_cloud_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
     def teardown_global(self):
         self.network.delete_network()
 
     @imports.inject("googleapiclient.errors", pip_extra="gcp")
     def authorize_gateways(errors, self, ips: List[str], rule_name: Optional[str] = None) -> str:
         firewall_name = f"skyplane-{uuid.uuid4().hex[:8]}" if rule_name is None else rule_name
+        self.network.create_firewall_rule(f"allow-default-{uuid.uuid4().hex[:8]}", "0.0.0.0/0", ["0-65535"], ["tcp"])
         self.network.create_firewall_rule(firewall_name, ips, ["0-65535"], ["tcp", "udp", "icmp"])
         return firewall_name
 
     @imports.inject("googleapiclient.errors", pip_extra="gcp")
     def remove_gateway_rule(errors, self, firewall_name: str):
         if self.network.get_firewall_rule(firewall_name):
             self.network.delete_firewall_rule(firewall_name)
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_key_manager.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_key_manager.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_network.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_network.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_pricing.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_pricing.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,28 +26,28 @@
                     raise Exception(f"Unknown continent {src_continent}")
             elif src.startswith("asia-southeast2") or src_continent == "australia":
                 return 0.15
             elif dst.startswith("asia-southeast2") or dst_continent == "australia":
                 return 0.15
             else:
                 return 0.08
-        elif dst_provider in ["aws", "azure"] and premium_tier:
+        elif dst_provider in ["aws", "azure", "cloudflare"] and premium_tier:
             is_dst_australia = (dst == "ap-southeast-2") if dst_provider == "aws" else (dst.startswith("australia"))
             # singapore or tokyo or osaka
             if src_continent == "asia" and (src_region == "southeast2" or src_region == "northeast1" or src_region == "northeast2"):
                 return 0.19 if is_dst_australia else 0.14
             # jakarta
             elif (src_continent == "asia" and src_region == "southeast1") or (src_continent == "australia"):
                 return 0.19
             # seoul
             elif src_continent == "asia" and src_region == "northeast3":
                 return 0.19 if is_dst_australia else 0.147
             else:
                 return 0.19 if is_dst_australia else 0.12
-        elif dst_provider in ["aws", "azure"] and not premium_tier:
+        elif dst_provider in ["aws", "azure", "cloudflare"] and not premium_tier:
             if src_continent == "us" or src_continent == "europe" or src_continent == "northamerica":
                 return 0.085
             elif src_continent == "southamerica" or src_continent == "australia":
                 return 0.12
             elif src_continent == "asia":
                 return 0.11
             else:
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/gcp/gcp_server.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/gcp/gcp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     @lru_cache(maxsize=1)
     def get_gcp_instance(self):
         instances = self.auth.get_gcp_instances(self.gcp_region)
         if "items" in instances:
             for i in instances["items"]:
                 if i["name"] == self.gcp_instance_name:
                     return i
-        raise ValueError(f"No instance found with name {self.gcp_instance_name}, {instances}")
+        raise ValueError(f"No instance found with name {self.gcp_instance_name}, {self.gcp_region}, {instances}")
 
     def get_instance_property(self, prop):
         instance = self.get_gcp_instance()
         if prop in instance:
             return instance[prop]
         else:
             return None
@@ -111,14 +111,15 @@
         import sshtunnel
 
         return sshtunnel.SSHTunnelForwarder(
             (self.public_ip(), 22),
             ssh_username=uname,
             ssh_pkey=str(self.ssh_private_key),
             ssh_private_key_password=ssh_key_password,
+            host_pkey_directories=[],
             local_bind_address=("127.0.0.1", 0),
             remote_bind_address=("127.0.0.1", remote_port),
         )
 
     def get_ssh_cmd(self, uname="skyplane", ssh_key_password="skyplane"):
         # todo can we include the key password inline?
         return f"ssh -i {self.ssh_private_key} -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no {uname}@{self.public_ip()}"
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/key_utils.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/key_utils.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/compute/server.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/compute/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import json
 import logging
+from pprint import pprint
 import os
 import socket
 from contextlib import closing
 from enum import Enum, auto
 from functools import partial
 from pathlib import Path
 
 import urllib3
 from typing import Dict, Optional, Tuple
 
 from skyplane import compute
 from skyplane.compute.const_cmds import make_autoshutdown_script, make_dozzle_command, make_sysctl_tcp_tuning_command
 from skyplane.config_paths import config_path, cloud_config, __config_root__
+from skyplane.gateway.gateway_program import GatewayProgram
 from skyplane.utils import logger
 from skyplane.utils.fn import PathLike, wait_for
 from skyplane.utils.retry import retry_backoff
 from skyplane.utils.timer import Timer
+from skyplane.planner.topology import TopologyPlanGateway
+
+tmp_log_dir = Path("/tmp/skyplane")
 
 
 class ServerState(Enum):
     PENDING = auto()
     RUNNING = auto()
     SUSPENDED = auto()
     TERMINATED = auto()
@@ -63,14 +68,26 @@
             "shutting-down": ServerState.TERMINATED,
             "terminated": ServerState.TERMINATED,
             "stopping": ServerState.SUSPENDED,
             "stopped": ServerState.SUSPENDED,
         }
         return mapping.get(aws_state, ServerState.UNKNOWN)
 
+    @staticmethod
+    def from_ibmcloud_state(ibmcloud_state):
+        mapping = {
+            "pending": ServerState.PENDING,
+            "running": ServerState.RUNNING,
+            "shutting-down": ServerState.TERMINATED,
+            "terminated": ServerState.TERMINATED,
+            "stopping": ServerState.SUSPENDED,
+            "stopped": ServerState.SUSPENDED,
+        }
+        return mapping.get(ibmcloud_state, ServerState.UNKNOWN)
+
 
 class Server:
     """Abstract server class to support basic SSH operations"""
 
     def __init__(self, region_tag, log_dir=None, auto_shutdown_timeout_minutes: Optional[int] = None):
         self.region_tag = region_tag  # format provider:region
         self.auto_shutdown_timeout_minutes = auto_shutdown_timeout_minutes
@@ -266,16 +283,17 @@
         if "Status: Downloaded newer image" not in docker_out and "Status: Image is up to date" not in docker_out:
             raise RuntimeError(
                 f"Failed to pull docker image {gateway_docker_image} on {self.region_tag}, {self.public_ip()}: OUT {docker_out}\nERR {docker_err}"
             )
 
     def start_gateway(
         self,
-        outgoing_ports: Dict[str, int],  # maps ip to number of connections along route
         gateway_docker_image: str,
+        gateway_program_path: str,
+        gateway_info_path: str,
         log_viewer_port=8888,
         use_bbr=False,
         use_compression=False,
         e2ee_key_bytes=None,
         use_socket_tls=False,
     ):
         def check_stderr(tup):
@@ -300,14 +318,15 @@
         if self.provider == "aws":
             docker_envs["AWS_METADATA_SERVICE_NUM_ATTEMPTS"] = "4"
             docker_envs["AWS_METADATA_SERVICE_TIMEOUT"] = "10"
 
         # pull docker image and start container
         with Timer() as t:
             retry_backoff(partial(self.pull_docker, gateway_docker_image), exception_class=RuntimeError)
+
         logger.fs.debug(f"{desc_prefix} docker pull in {t.elapsed}")
         logger.fs.debug(f"{desc_prefix}: Starting gateway container")
         docker_run_flags = f"-d --log-driver=local --log-opt max-file=16 --ipc=host --network=host --ulimit nofile={1024 * 1024}"
         docker_run_flags += " --mount type=tmpfs,dst=/skyplane,tmpfs-size=$(($(free -b  | head -n2 | tail -n1 | awk '{print $2}')/2))"
         docker_run_flags += f" -v /tmp/{config_path.name}:/pkg/data/{config_path.name}"
 
         # copy service account files
@@ -325,17 +344,28 @@
         # copy E2EE keys
         if e2ee_key_bytes is not None:
             e2ee_key_file = "e2ee_key"
             self.write_file(e2ee_key_bytes, f"/tmp/{e2ee_key_file}")
             docker_envs["E2EE_KEY_FILE"] = f"/pkg/data/{e2ee_key_file}"
             docker_run_flags += f" -v /tmp/{e2ee_key_file}:/pkg/data/{e2ee_key_file}"
 
-        docker_run_flags += " " + " ".join(f"--env {k}={v}" for k, v in docker_envs.items())
+        # upload gateway programs and gateway info
+        gateway_program_file = os.path.basename(gateway_program_path).replace(":", "_")
+        gateway_info_file = os.path.basename(gateway_info_path).replace(":", "_")
+        self.upload_file(gateway_program_path, f"/tmp/{gateway_program_file}")  # upload gateway program
+        self.upload_file(gateway_info_path, f"/tmp/{gateway_info_file}")  # upload gateway info
+        docker_envs["GATEWAY_PROGRAM_FILE"] = f"/pkg/data/gateway_program.json"
+        docker_envs["GATEWAY_INFO_FILE"] = f"/pkg/data/gateway_info.json"
+        docker_run_flags += f" -v /tmp/{gateway_program_file}:/pkg/data/gateway_program.json"
+        docker_run_flags += f" -v /tmp/{gateway_info_file}:/pkg/data/gateway_info.json"
         gateway_daemon_cmd = f"/etc/init.d/stunnel4 start && python -u /pkg/skyplane/gateway/gateway_daemon.py --chunk-dir /skyplane/chunks"
-        gateway_daemon_cmd += f" --outgoing-ports '{json.dumps(outgoing_ports)}'"
+
+        # update docker flags
+        docker_run_flags += " " + " ".join(f"--env {k}={v}" for k, v in docker_envs.items())
+
         gateway_daemon_cmd += f" --region {self.region_tag} {'--use-compression' if use_compression else ''}"
         gateway_daemon_cmd += f" {'--disable-e2ee' if e2ee_key_bytes is None else ''}"
         gateway_daemon_cmd += f" {'--disable-tls' if not use_socket_tls else ''}"
         escaped_gateway_daemon_cmd = gateway_daemon_cmd.replace('"', '\\"')
         docker_launch_cmd = (
             f'sudo docker run {docker_run_flags} --name skyplane_gateway {gateway_docker_image} /bin/bash -c "{escaped_gateway_daemon_cmd}"'
         )
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/config_paths.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/config_paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import functools
 import os
 from pathlib import Path
 
 
 __config_root__ = Path("~/.skyplane").expanduser()
 aws_config_path = __config_root__ / "aws_config"
+aws_quota_path = __config_root__ / "aws_quota"
 azure_config_path = __config_root__ / "azure_config"
+azure_quota_path = __config_root__ / "azure_quota"
+azure_standardDv5_quota_path = __config_root__ / "azure_standardDv5_quota"
 azure_sku_path = __config_root__ / "azure_sku_mapping"
 gcp_config_path = __config_root__ / "gcp_config"
+ibmcloud_config_path = __config_root__ / "ibmcloud_config"
+gcp_quota_path = __config_root__ / "gcp_quota"
 
 
 @functools.lru_cache(maxsize=None)
 def load_config_path():
     if "SKYPLANE_CONFIG" in os.environ:
         path = Path(os.environ["SKYPLANE_CONFIG"]).expanduser()
     else:
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/data/aws_transfer_costs.csv` & `skyplane_nightly-0.3.2.dev20230622/skyplane/data/aws_transfer_costs.csv`

 * *Files 23% similar despite different names*

```diff
@@ -1,529 +1,675 @@
-src,dst,cost
-us-gov-east-1,internet,0.155
-us-gov-east-1,af-south-1,0.03
-us-gov-east-1,ap-east-1,0.03
-us-gov-east-1,ap-southeast-3,0.03
-us-gov-east-1,ap-south-1,0.03
-us-gov-east-1,ap-northeast-3,0.03
-us-gov-east-1,ap-northeast-2,0.03
-us-gov-east-1,ap-southeast-1,0.03
-us-gov-east-1,ap-southeast-2,0.03
-us-gov-east-1,ap-northeast-1,0.03
-us-gov-east-1,ca-central-1,0.03
-us-gov-east-1,eu-central-1,0.03
-us-gov-east-1,eu-west-1,0.03
-us-gov-east-1,eu-west-2,0.03
-us-gov-east-1,eu-south-1,0.03
-us-gov-east-1,eu-west-3,0.03
-us-gov-east-1,eu-north-1,0.03
-us-gov-east-1,me-south-1,0.03
-us-gov-east-1,sa-east-1,0.03
-us-gov-east-1,us-east-1,0.03
-us-gov-east-1,us-east-2,0.03
-us-gov-east-1,us-west-1,0.03
-us-gov-east-1,us-west-2,0.03
-af-south-1,internet,0.154
-af-south-1,us-gov-east-1,0.147
-af-south-1,ap-east-1,0.147
-af-south-1,ap-southeast-3,0.147
-af-south-1,ap-south-1,0.147
-af-south-1,ap-northeast-3,0.147
-af-south-1,ap-northeast-2,0.147
-af-south-1,ap-southeast-1,0.147
-af-south-1,ap-southeast-2,0.147
-af-south-1,ap-northeast-1,0.147
-af-south-1,ca-central-1,0.147
-af-south-1,eu-central-1,0.147
-af-south-1,eu-west-1,0.147
-af-south-1,eu-west-2,0.147
-af-south-1,eu-south-1,0.147
-af-south-1,eu-west-3,0.147
-af-south-1,eu-north-1,0.147
-af-south-1,me-south-1,0.147
-af-south-1,sa-east-1,0.147
-af-south-1,us-east-1,0.147
-af-south-1,us-east-2,0.147
-af-south-1,us-west-1,0.147
-af-south-1,us-west-2,0.147
-ap-east-1,internet,0.12
-ap-east-1,us-gov-east-1,0.09
-ap-east-1,af-south-1,0.09
-ap-east-1,ap-southeast-3,0.09
-ap-east-1,ap-south-1,0.09
-ap-east-1,ap-northeast-3,0.09
-ap-east-1,ap-northeast-2,0.09
-ap-east-1,ap-southeast-1,0.09
-ap-east-1,ap-southeast-2,0.09
-ap-east-1,ap-northeast-1,0.09
-ap-east-1,ca-central-1,0.09
-ap-east-1,eu-central-1,0.09
-ap-east-1,eu-west-1,0.09
-ap-east-1,eu-west-2,0.09
-ap-east-1,eu-south-1,0.09
-ap-east-1,eu-west-3,0.09
-ap-east-1,eu-north-1,0.09
-ap-east-1,me-south-1,0.09
-ap-east-1,sa-east-1,0.09
-ap-east-1,us-east-1,0.09
-ap-east-1,us-east-2,0.09
-ap-east-1,us-west-1,0.09
-ap-east-1,us-west-2,0.09
-ap-southeast-3,internet,0.132
-ap-southeast-3,us-gov-east-1,0.1
-ap-southeast-3,af-south-1,0.1
-ap-southeast-3,ap-east-1,0.1
-ap-southeast-3,ap-southeast-3,0.1
-ap-southeast-3,ap-northeast-3,0.1
-ap-southeast-3,ap-northeast-2,0.1
-ap-southeast-3,ap-southeast-1,0.1
-ap-southeast-3,ap-southeast-2,0.1
-ap-southeast-3,ap-northeast-1,0.1
-ap-southeast-3,ca-central-1,0.1
-ap-southeast-3,eu-central-1,0.1
-ap-southeast-3,eu-west-1,0.1
-ap-southeast-3,eu-west-2,0.1
-ap-southeast-3,eu-south-1,0.1
-ap-southeast-3,eu-west-3,0.1
-ap-southeast-3,eu-north-1,0.1
-ap-southeast-3,me-south-1,0.1
-ap-southeast-3,sa-east-1,0.1
-ap-southeast-3,us-east-1,0.1
-ap-southeast-3,us-east-2,0.1
-ap-southeast-3,us-west-1,0.1
-ap-southeast-3,us-west-2,0.1
-ap-south-1,internet,0.1093
-ap-south-1,us-gov-east-1,0.086
-ap-south-1,af-south-1,0.086
-ap-south-1,ap-east-1,0.086
-ap-south-1,ap-southeast-3,0.086
-ap-south-1,ap-northeast-3,0.086
-ap-south-1,ap-northeast-2,0.086
-ap-south-1,ap-southeast-1,0.086
-ap-south-1,ap-southeast-2,0.086
-ap-south-1,ap-northeast-1,0.086
-ap-south-1,ca-central-1,0.086
-ap-south-1,eu-central-1,0.086
-ap-south-1,eu-west-1,0.086
-ap-south-1,eu-west-2,0.086
-ap-south-1,eu-south-1,0.086
-ap-south-1,eu-west-3,0.086
-ap-south-1,eu-north-1,0.086
-ap-south-1,me-south-1,0.086
-ap-south-1,sa-east-1,0.086
-ap-south-1,us-east-1,0.086
-ap-south-1,us-east-2,0.086
-ap-south-1,us-west-1,0.086
-ap-south-1,us-west-2,0.086
-ap-northeast-3,internet,0.114
-ap-northeast-3,us-gov-east-1,0.09
-ap-northeast-3,af-south-1,0.09
-ap-northeast-3,ap-east-1,0.09
-ap-northeast-3,ap-southeast-3,0.09
-ap-northeast-3,ap-south-1,0.09
-ap-northeast-3,ap-northeast-2,0.09
-ap-northeast-3,ap-southeast-1,0.09
-ap-northeast-3,ap-southeast-2,0.09
-ap-northeast-3,ap-northeast-1,0.09
-ap-northeast-3,ca-central-1,0.09
-ap-northeast-3,eu-central-1,0.09
-ap-northeast-3,eu-west-1,0.09
-ap-northeast-3,eu-west-2,0.09
-ap-northeast-3,eu-south-1,0.09
-ap-northeast-3,eu-west-3,0.09
-ap-northeast-3,eu-north-1,0.09
-ap-northeast-3,me-south-1,0.09
-ap-northeast-3,sa-east-1,0.09
-ap-northeast-3,us-east-1,0.09
-ap-northeast-3,us-east-2,0.09
-ap-northeast-3,us-west-1,0.09
-ap-northeast-3,us-west-2,0.09
-ap-northeast-2,internet,0.126
-ap-northeast-2,us-gov-east-1,0.08
-ap-northeast-2,af-south-1,0.08
-ap-northeast-2,ap-east-1,0.08
-ap-northeast-2,ap-southeast-3,0.08
-ap-northeast-2,ap-south-1,0.08
-ap-northeast-2,ap-northeast-3,0.08
-ap-northeast-2,ap-southeast-1,0.08
-ap-northeast-2,ap-southeast-2,0.08
-ap-northeast-2,ap-northeast-1,0.08
-ap-northeast-2,ca-central-1,0.08
-ap-northeast-2,eu-central-1,0.08
-ap-northeast-2,eu-west-1,0.08
-ap-northeast-2,eu-west-2,0.08
-ap-northeast-2,eu-south-1,0.08
-ap-northeast-2,eu-west-3,0.08
-ap-northeast-2,eu-north-1,0.08
-ap-northeast-2,me-south-1,0.08
-ap-northeast-2,sa-east-1,0.08
-ap-northeast-2,us-east-1,0.08
-ap-northeast-2,us-east-2,0.08
-ap-northeast-2,us-west-1,0.08
-ap-northeast-2,us-west-2,0.08
-ap-southeast-1,internet,0.12
-ap-southeast-1,us-gov-east-1,0.09
-ap-southeast-1,af-south-1,0.09
-ap-southeast-1,ap-east-1,0.09
-ap-southeast-1,ap-south-1,0.09
-ap-southeast-1,ap-northeast-3,0.09
-ap-southeast-1,ap-northeast-2,0.09
-ap-southeast-1,ap-southeast-2,0.09
-ap-southeast-1,ap-northeast-1,0.09
-ap-southeast-1,ca-central-1,0.09
-ap-southeast-1,eu-central-1,0.09
-ap-southeast-1,eu-west-1,0.09
-ap-southeast-1,eu-west-2,0.09
-ap-southeast-1,eu-south-1,0.09
-ap-southeast-1,eu-west-3,0.09
-ap-southeast-1,eu-north-1,0.09
-ap-southeast-1,me-south-1,0.09
-ap-southeast-1,sa-east-1,0.09
-ap-southeast-1,us-east-1,0.09
-ap-southeast-1,us-east-2,0.09
-ap-southeast-1,us-west-1,0.09
-ap-southeast-1,us-west-2,0.09
-ap-southeast-2,internet,0.114
-ap-southeast-2,us-gov-east-1,0.098
-ap-southeast-2,af-south-1,0.098
-ap-southeast-2,ap-east-1,0.098
-ap-southeast-2,ap-southeast-3,0.098
-ap-southeast-2,ap-south-1,0.098
-ap-southeast-2,ap-northeast-3,0.098
-ap-southeast-2,ap-northeast-2,0.098
-ap-southeast-2,ap-southeast-1,0.098
-ap-southeast-2,ap-northeast-1,0.098
-ap-southeast-2,ca-central-1,0.098
-ap-southeast-2,eu-central-1,0.098
-ap-southeast-2,eu-west-1,0.098
-ap-southeast-2,eu-west-2,0.098
-ap-southeast-2,eu-south-1,0.098
-ap-southeast-2,eu-west-3,0.098
-ap-southeast-2,eu-north-1,0.098
-ap-southeast-2,me-south-1,0.098
-ap-southeast-2,sa-east-1,0.098
-ap-southeast-2,us-east-1,0.098
-ap-southeast-2,us-east-2,0.098
-ap-southeast-2,us-west-1,0.098
-ap-southeast-2,us-west-2,0.098
-ap-northeast-1,internet,0.114
-ap-northeast-1,us-gov-east-1,0.09
-ap-northeast-1,af-south-1,0.09
-ap-northeast-1,ap-east-1,0.09
-ap-northeast-1,ap-southeast-3,0.09
-ap-northeast-1,ap-south-1,0.09
-ap-northeast-1,ap-northeast-3,0.09
-ap-northeast-1,ap-northeast-2,0.09
-ap-northeast-1,ap-southeast-1,0.09
-ap-northeast-1,ap-southeast-2,0.09
-ap-northeast-1,ca-central-1,0.09
-ap-northeast-1,eu-central-1,0.09
-ap-northeast-1,eu-west-1,0.09
-ap-northeast-1,eu-west-2,0.09
-ap-northeast-1,eu-south-1,0.09
-ap-northeast-1,eu-west-3,0.09
-ap-northeast-1,eu-north-1,0.09
-ap-northeast-1,me-south-1,0.09
-ap-northeast-1,sa-east-1,0.09
-ap-northeast-1,us-east-1,0.09
-ap-northeast-1,us-east-2,0.09
-ap-northeast-1,us-west-1,0.09
-ap-northeast-1,us-west-2,0.09
-ca-central-1,internet,0.09
-ca-central-1,us-gov-east-1,0.02
-ca-central-1,af-south-1,0.02
-ca-central-1,ap-east-1,0.02
-ca-central-1,ap-southeast-3,0.02
-ca-central-1,ap-south-1,0.02
-ca-central-1,ap-northeast-3,0.02
-ca-central-1,ap-northeast-2,0.02
-ca-central-1,ap-southeast-1,0.02
-ca-central-1,ap-southeast-2,0.02
-ca-central-1,ap-northeast-1,0.02
-ca-central-1,eu-central-1,0.02
-ca-central-1,eu-west-1,0.02
-ca-central-1,eu-west-2,0.02
-ca-central-1,eu-south-1,0.02
-ca-central-1,eu-west-3,0.02
-ca-central-1,eu-north-1,0.02
-ca-central-1,me-south-1,0.02
-ca-central-1,sa-east-1,0.02
-ca-central-1,us-east-1,0.02
-ca-central-1,us-east-2,0.02
-ca-central-1,us-west-1,0.02
-ca-central-1,us-west-2,0.02
-eu-central-1,internet,0.09
-eu-central-1,us-gov-east-1,0.02
-eu-central-1,af-south-1,0.02
-eu-central-1,ap-east-1,0.02
-eu-central-1,ap-south-1,0.02
-eu-central-1,ap-northeast-3,0.02
-eu-central-1,ap-northeast-2,0.02
-eu-central-1,ap-southeast-1,0.02
-eu-central-1,ap-southeast-2,0.02
-eu-central-1,ap-southeast-3,0.02
-eu-central-1,ap-northeast-1,0.02
-eu-central-1,ca-central-1,0.02
-eu-central-1,eu-west-1,0.02
-eu-central-1,eu-west-2,0.02
-eu-central-1,eu-south-1,0.02
-eu-central-1,eu-west-3,0.02
-eu-central-1,eu-north-1,0.02
-eu-central-1,me-south-1,0.02
-eu-central-1,sa-east-1,0.02
-eu-central-1,us-east-1,0.02
-eu-central-1,us-east-2,0.02
-eu-central-1,us-west-1,0.02
-eu-central-1,us-west-2,0.02
-eu-west-1,internet,0.09
-eu-west-1,us-gov-east-1,0.02
-eu-west-1,af-south-1,0.02
-eu-west-1,ap-east-1,0.02
-eu-west-1,ap-southeast-3,0.02
-eu-west-1,ap-south-1,0.02
-eu-west-1,ap-northeast-3,0.02
-eu-west-1,ap-northeast-2,0.02
-eu-west-1,ap-southeast-1,0.02
-eu-west-1,ap-southeast-2,0.02
-eu-west-1,ap-northeast-1,0.02
-eu-west-1,ca-central-1,0.02
-eu-west-1,eu-central-1,0.02
-eu-west-1,eu-west-2,0.02
-eu-west-1,eu-south-1,0.02
-eu-west-1,eu-west-3,0.02
-eu-west-1,eu-north-1,0.02
-eu-west-1,me-south-1,0.02
-eu-west-1,sa-east-1,0.02
-eu-west-1,us-east-1,0.02
-eu-west-1,us-east-2,0.02
-eu-west-1,us-west-1,0.02
-eu-west-1,us-west-2,0.02
-eu-west-2,internet,0.09
-eu-west-2,us-gov-east-1,0.02
-eu-west-2,af-south-1,0.02
-eu-west-2,ap-east-1,0.02
-eu-west-2,ap-southeast-3,0.02
-eu-west-2,ap-south-1,0.02
-eu-west-2,ap-northeast-3,0.02
-eu-west-2,ap-northeast-2,0.02
-eu-west-2,ap-southeast-1,0.02
-eu-west-2,ap-southeast-2,0.02
-eu-west-2,ap-northeast-1,0.02
-eu-west-2,ca-central-1,0.02
-eu-west-2,eu-central-1,0.02
-eu-west-2,eu-west-1,0.02
-eu-west-2,eu-south-1,0.02
-eu-west-2,eu-west-3,0.02
-eu-west-2,eu-north-1,0.02
-eu-west-2,me-south-1,0.02
-eu-west-2,sa-east-1,0.02
-eu-west-2,us-east-1,0.02
-eu-west-2,us-east-2,0.02
-eu-west-2,us-west-1,0.02
-eu-west-2,us-west-2,0.02
-eu-south-1,internet,0.09
-eu-south-1,us-gov-east-1,0.02
-eu-south-1,af-south-1,0.02
-eu-south-1,ap-east-1,0.02
-eu-south-1,ap-southeast-3,0.02
-eu-south-1,ap-south-1,0.02
-eu-south-1,ap-northeast-3,0.02
-eu-south-1,ap-northeast-2,0.02
-eu-south-1,ap-southeast-1,0.02
-eu-south-1,ap-southeast-2,0.02
-eu-south-1,ap-northeast-1,0.02
-eu-south-1,ca-central-1,0.02
-eu-south-1,eu-central-1,0.02
-eu-south-1,eu-west-1,0.02
-eu-south-1,eu-west-2,0.02
-eu-south-1,eu-west-3,0.02
-eu-south-1,eu-north-1,0.02
-eu-south-1,me-south-1,0.02
-eu-south-1,sa-east-1,0.02
-eu-south-1,us-east-1,0.02
-eu-south-1,us-east-2,0.02
-eu-south-1,us-west-1,0.02
-eu-south-1,us-west-2,0.02
-eu-west-3,internet,0.09
-eu-west-3,us-gov-east-1,0.02
-eu-west-3,af-south-1,0.02
-eu-west-3,ap-east-1,0.02
-eu-west-3,ap-southeast-3,0.02
-eu-west-3,ap-south-1,0.02
-eu-west-3,ap-northeast-3,0.02
-eu-west-3,ap-northeast-2,0.02
-eu-west-3,ap-southeast-1,0.02
-eu-west-3,ap-southeast-2,0.02
-eu-west-3,ap-northeast-1,0.02
-eu-west-3,ca-central-1,0.02
-eu-west-3,eu-central-1,0.02
-eu-west-3,eu-west-1,0.02
-eu-west-3,eu-west-2,0.02
-eu-west-3,eu-south-1,0.02
-eu-west-3,eu-north-1,0.02
-eu-west-3,me-south-1,0.02
-eu-west-3,sa-east-1,0.02
-eu-west-3,us-east-1,0.02
-eu-west-3,us-east-2,0.02
-eu-west-3,us-west-1,0.02
-eu-west-3,us-west-2,0.02
-eu-north-1,internet,0.09
-eu-north-1,us-gov-east-1,0.02
-eu-north-1,af-south-1,0.02
-eu-north-1,ap-east-1,0.02
-eu-north-1,ap-southeast-3,0.02
-eu-north-1,ap-south-1,0.02
-eu-north-1,ap-northeast-3,0.02
-eu-north-1,ap-northeast-2,0.02
-eu-north-1,ap-southeast-1,0.02
-eu-north-1,ap-southeast-2,0.02
-eu-north-1,ap-northeast-1,0.02
-eu-north-1,ca-central-1,0.02
-eu-north-1,eu-central-1,0.02
-eu-north-1,eu-west-1,0.02
-eu-north-1,eu-west-2,0.02
-eu-north-1,eu-south-1,0.02
-eu-north-1,eu-west-3,0.02
-eu-north-1,me-south-1,0.02
-eu-north-1,sa-east-1,0.02
-eu-north-1,us-east-1,0.02
-eu-north-1,us-east-2,0.02
-eu-north-1,us-west-1,0.02
-eu-north-1,us-west-2,0.02
-me-south-1,internet,0.117
-me-south-1,us-gov-east-1,0.1105
-me-south-1,af-south-1,0.1105
-me-south-1,ap-east-1,0.1105
-me-south-1,ap-southeast-3,0.1105
-me-south-1,ap-south-1,0.1105
-me-south-1,ap-northeast-3,0.1105
-me-south-1,ap-northeast-2,0.1105
-me-south-1,ap-southeast-1,0.1105
-me-south-1,ap-southeast-2,0.1105
-me-south-1,ap-northeast-1,0.1105
-me-south-1,ca-central-1,0.1105
-me-south-1,eu-central-1,0.1105
-me-south-1,eu-west-1,0.1105
-me-south-1,eu-west-2,0.1105
-me-south-1,eu-south-1,0.1105
-me-south-1,eu-west-3,0.1105
-me-south-1,eu-north-1,0.1105
-me-south-1,sa-east-1,0.1105
-me-south-1,us-east-1,0.1105
-me-south-1,us-east-2,0.1105
-me-south-1,us-west-1,0.1105
-me-south-1,us-west-2,0.1105
-sa-east-1,internet,0.15
-sa-east-1,us-gov-east-1,0.138
-sa-east-1,af-south-1,0.138
-sa-east-1,ap-east-1,0.138
-sa-east-1,ap-southeast-3,0.138
-sa-east-1,ap-south-1,0.138
-sa-east-1,ap-northeast-3,0.138
-sa-east-1,ap-northeast-2,0.138
-sa-east-1,ap-southeast-1,0.138
-sa-east-1,ap-southeast-2,0.138
-sa-east-1,ap-northeast-1,0.138
-sa-east-1,ca-central-1,0.138
-sa-east-1,eu-central-1,0.138
-sa-east-1,eu-west-1,0.138
-sa-east-1,eu-west-2,0.138
-sa-east-1,eu-south-1,0.138
-sa-east-1,eu-west-3,0.138
-sa-east-1,eu-north-1,0.138
-sa-east-1,me-south-1,0.138
-sa-east-1,us-east-1,0.138
-sa-east-1,us-east-2,0.138
-sa-east-1,us-west-1,0.138
-sa-east-1,us-west-2,0.138
-us-east-1,internet,0.09
-us-east-1,us-gov-east-1,0.02
-us-east-1,af-south-1,0.02
-us-east-1,ap-east-1,0.02
-us-east-1,ap-southeast-3,0.02
-us-east-1,ap-south-1,0.02
-us-east-1,ap-northeast-3,0.02
-us-east-1,ap-northeast-2,0.02
-us-east-1,ap-southeast-1,0.02
-us-east-1,ap-southeast-2,0.02
-us-east-1,ap-northeast-1,0.02
-us-east-1,ca-central-1,0.02
-us-east-1,eu-central-1,0.02
-us-east-1,eu-west-1,0.02
-us-east-1,eu-west-2,0.02
-us-east-1,eu-south-1,0.02
-us-east-1,eu-west-3,0.02
-us-east-1,eu-north-1,0.02
-us-east-1,me-south-1,0.02
-us-east-1,sa-east-1,0.02
-us-east-1,us-east-2,0.01
-us-east-1,us-west-1,0.02
-us-east-1,us-west-2,0.02
-us-east-2,internet,0.09
-us-east-2,us-gov-east-1,0.02
-us-east-2,af-south-1,0.02
-us-east-2,ap-east-1,0.02
-us-east-2,ap-southeast-3,0.02
-us-east-2,ap-south-1,0.02
-us-east-2,ap-northeast-3,0.02
-us-east-2,ap-northeast-2,0.02
-us-east-2,ap-southeast-1,0.02
-us-east-2,ap-southeast-2,0.02
-us-east-2,ap-northeast-1,0.02
-us-east-2,ca-central-1,0.02
-us-east-2,eu-central-1,0.02
-us-east-2,eu-west-1,0.02
-us-east-2,eu-west-2,0.02
-us-east-2,eu-south-1,0.02
-us-east-2,eu-west-3,0.02
-us-east-2,eu-north-1,0.02
-us-east-2,me-south-1,0.02
-us-east-2,sa-east-1,0.02
-us-east-2,us-east-1,0.01
-us-east-2,us-west-1,0.02
-us-east-2,us-west-2,0.02
-us-west-1,internet,0.09
-us-west-1,us-gov-east-1,0.02
-us-west-1,af-south-1,0.02
-us-west-1,ap-east-1,0.02
-us-west-1,ap-southeast-3,0.02
-us-west-1,ap-south-1,0.02
-us-west-1,ap-northeast-3,0.02
-us-west-1,ap-northeast-2,0.02
-us-west-1,ap-southeast-1,0.02
-us-west-1,ap-southeast-2,0.02
-us-west-1,ap-northeast-1,0.02
-us-west-1,ca-central-1,0.02
-us-west-1,eu-central-1,0.02
-us-west-1,eu-west-1,0.02
-us-west-1,eu-west-2,0.02
-us-west-1,eu-south-1,0.02
-us-west-1,eu-west-3,0.02
-us-west-1,eu-north-1,0.02
-us-west-1,me-south-1,0.02
-us-west-1,sa-east-1,0.02
-us-west-1,us-east-1,0.02
-us-west-1,us-east-2,0.02
-us-west-1,us-west-2,0.02
-us-west-2,internet,0.09
-us-west-2,us-gov-east-1,0.02
-us-west-2,af-south-1,0.02
-us-west-2,ap-east-1,0.02
-us-west-2,ap-southeast-3,0.02
-us-west-2,ap-south-1,0.02
-us-west-2,ap-northeast-3,0.02
-us-west-2,ap-northeast-2,0.02
-us-west-2,ap-southeast-1,0.02
-us-west-2,ap-southeast-2,0.02
-us-west-2,ap-northeast-1,0.02
-us-west-2,ca-central-1,0.02
-us-west-2,eu-central-1,0.02
-us-west-2,eu-west-1,0.02
-us-west-2,eu-west-2,0.02
-us-west-2,eu-south-1,0.02
-us-west-2,eu-west-3,0.02
-us-west-2,eu-north-1,0.02
-us-west-2,me-south-1,0.02
-us-west-2,sa-east-1,0.02
-us-west-2,us-east-1,0.02
-us-west-2,us-east-2,0.02
-us-west-2,us-west-1,0.02
+src,dst,cost
+us-gov-east-1,internet,0.155
+us-gov-east-1,af-south-1,0.03
+us-gov-east-1,ap-east-1,0.03
+us-gov-east-1,ap-southeast-3,0.03
+us-gov-east-1,ap-south-1,0.03
+us-gov-east-1,ap-northeast-3,0.03
+us-gov-east-1,ap-northeast-2,0.03
+us-gov-east-1,ap-southeast-1,0.03
+us-gov-east-1,ap-southeast-2,0.03
+us-gov-east-1,ap-northeast-1,0.03
+us-gov-east-1,ca-central-1,0.03
+us-gov-east-1,eu-central-1,0.03
+us-gov-east-1,eu-west-1,0.03
+us-gov-east-1,eu-west-2,0.03
+us-gov-east-1,eu-south-1,0.03
+us-gov-east-1,eu-west-3,0.03
+us-gov-east-1,eu-south-2,0.03
+us-gov-east-1,eu-north-1,0.03
+us-gov-east-1,eu-central-2,0.03
+us-gov-east-1,me-south-1,0.03
+us-gov-east-1,me-central-1,0.03
+us-gov-east-1,sa-east-1,0.03
+us-gov-east-1,us-east-1,0.03
+us-gov-east-1,us-east-2,0.03
+us-gov-east-1,us-west-1,0.03
+us-gov-east-1,us-west-2,0.03
+af-south-1,internet,0.154
+af-south-1,us-gov-east-1,0.147
+af-south-1,ap-east-1,0.147
+af-south-1,ap-southeast-3,0.147
+af-south-1,ap-south-1,0.147
+af-south-1,ap-northeast-3,0.147
+af-south-1,ap-northeast-2,0.147
+af-south-1,ap-southeast-1,0.147
+af-south-1,ap-southeast-2,0.147
+af-south-1,ap-northeast-1,0.147
+af-south-1,ca-central-1,0.147
+af-south-1,eu-central-1,0.147
+af-south-1,eu-west-1,0.147
+af-south-1,eu-west-2,0.147
+af-south-1,eu-south-1,0.147
+af-south-1,eu-west-3,0.147
+af-south-1,eu-south-2,0.147
+af-south-1,eu-north-1,0.147
+af-south-1,eu-central-2,0.147
+af-south-1,me-south-1,0.147
+af-south-1,me-central-1,0.147
+af-south-1,sa-east-1,0.147
+af-south-1,us-east-1,0.147
+af-south-1,us-east-2,0.147
+af-south-1,us-west-1,0.147
+af-south-1,us-west-2,0.147
+ap-east-1,internet,0.12
+ap-east-1,us-gov-east-1,0.09
+ap-east-1,af-south-1,0.09
+ap-east-1,ap-southeast-3,0.09
+ap-east-1,ap-south-1,0.09
+ap-east-1,ap-northeast-3,0.09
+ap-east-1,ap-northeast-2,0.09
+ap-east-1,ap-southeast-1,0.09
+ap-east-1,ap-southeast-2,0.09
+ap-east-1,ap-northeast-1,0.09
+ap-east-1,ca-central-1,0.09
+ap-east-1,eu-central-1,0.09
+ap-east-1,eu-west-1,0.09
+ap-east-1,eu-west-2,0.09
+ap-east-1,eu-south-1,0.09
+ap-east-1,eu-west-3,0.09
+ap-east-1,eu-south-2,0.09
+ap-east-1,eu-north-1,0.09
+ap-east-1,eu-central-2,0.09
+ap-east-1,me-south-1,0.09
+ap-east-1,me-central-1,0.09
+ap-east-1,sa-east-1,0.09
+ap-east-1,us-east-1,0.09
+ap-east-1,us-east-2,0.09
+ap-east-1,us-west-1,0.09
+ap-east-1,us-west-2,0.09
+ap-southeast-3,internet,0.132
+ap-southeast-3,us-gov-east-1,0.1
+ap-southeast-3,af-south-1,0.1
+ap-southeast-3,ap-east-1,0.1
+ap-southeast-3,ap-south-1,0.1
+ap-southeast-3,ap-northeast-2,0.1
+ap-southeast-3,ap-southeast-1,0.1
+ap-southeast-3,ap-southeast-2,0.1
+ap-southeast-3,ap-northeast-1,0.1
+ap-southeast-3,ca-central-1,0.1
+ap-southeast-3,eu-central-1,0.1
+ap-southeast-3,eu-west-1,0.1
+ap-southeast-3,eu-west-2,0.1
+ap-southeast-3,eu-south-1,0.1
+ap-southeast-3,eu-west-3,0.1
+ap-southeast-3,eu-south-2,0.1
+ap-southeast-3,eu-north-1,0.1
+ap-southeast-3,eu-central-2,0.1
+ap-southeast-3,me-south-1,0.1
+ap-southeast-3,me-central-1,0.1
+ap-southeast-3,us-east-1,0.1
+ap-southeast-3,us-east-2,0.1
+ap-southeast-3,us-west-1,0.1
+ap-southeast-3,us-west-2,0.1
+ap-south-1,internet,0.1093
+ap-south-1,us-gov-east-1,0.086
+ap-south-1,af-south-1,0.086
+ap-south-1,ap-east-1,0.086
+ap-south-1,ap-southeast-3,0.086
+ap-south-1,ap-northeast-3,0.086
+ap-south-1,ap-northeast-2,0.086
+ap-south-1,ap-southeast-1,0.086
+ap-south-1,ap-southeast-2,0.086
+ap-south-1,ap-northeast-1,0.086
+ap-south-1,ca-central-1,0.086
+ap-south-1,eu-central-1,0.086
+ap-south-1,eu-west-1,0.086
+ap-south-1,eu-west-2,0.086
+ap-south-1,eu-south-1,0.086
+ap-south-1,eu-west-3,0.086
+ap-south-1,eu-south-2,0.086
+ap-south-1,eu-north-1,0.086
+ap-south-1,eu-central-2,0.086
+ap-south-1,me-south-1,0.086
+ap-south-1,me-central-1,0.086
+ap-south-1,sa-east-1,0.086
+ap-south-1,us-east-1,0.086
+ap-south-1,us-east-2,0.086
+ap-south-1,us-west-1,0.086
+ap-south-1,us-west-2,0.086
+ap-northeast-3,internet,0.114
+ap-northeast-3,us-gov-east-1,0.09
+ap-northeast-3,af-south-1,0.09
+ap-northeast-3,ap-east-1,0.09
+ap-northeast-3,ap-southeast-3,0.09
+ap-northeast-3,ap-south-1,0.09
+ap-northeast-3,ap-northeast-2,0.09
+ap-northeast-3,ap-southeast-1,0.09
+ap-northeast-3,ap-southeast-2,0.09
+ap-northeast-3,ap-northeast-1,0.09
+ap-northeast-3,ca-central-1,0.09
+ap-northeast-3,eu-central-1,0.09
+ap-northeast-3,eu-west-1,0.09
+ap-northeast-3,eu-west-2,0.09
+ap-northeast-3,eu-south-1,0.09
+ap-northeast-3,eu-west-3,0.09
+ap-northeast-3,eu-south-2,0.09
+ap-northeast-3,eu-north-1,0.09
+ap-northeast-3,eu-central-2,0.09
+ap-northeast-3,me-south-1,0.09
+ap-northeast-3,me-central-1,0.09
+ap-northeast-3,sa-east-1,0.09
+ap-northeast-3,us-east-1,0.09
+ap-northeast-3,us-east-2,0.09
+ap-northeast-3,us-west-1,0.09
+ap-northeast-3,us-west-2,0.09
+ap-northeast-2,internet,0.126
+ap-northeast-2,us-gov-east-1,0.08
+ap-northeast-2,af-south-1,0.08
+ap-northeast-2,ap-east-1,0.08
+ap-northeast-2,ap-southeast-3,0.08
+ap-northeast-2,ap-south-1,0.08
+ap-northeast-2,ap-northeast-3,0.08
+ap-northeast-2,ap-southeast-1,0.08
+ap-northeast-2,ap-southeast-2,0.08
+ap-northeast-2,ap-northeast-1,0.08
+ap-northeast-2,ca-central-1,0.08
+ap-northeast-2,eu-central-1,0.08
+ap-northeast-2,eu-west-1,0.08
+ap-northeast-2,eu-west-2,0.08
+ap-northeast-2,eu-south-1,0.08
+ap-northeast-2,eu-west-3,0.08
+ap-northeast-2,eu-south-2,0.08
+ap-northeast-2,eu-north-1,0.08
+ap-northeast-2,eu-central-2,0.08
+ap-northeast-2,me-south-1,0.08
+ap-northeast-2,me-central-1,0.08
+ap-northeast-2,sa-east-1,0.08
+ap-northeast-2,us-east-1,0.08
+ap-northeast-2,us-east-2,0.08
+ap-northeast-2,us-west-1,0.08
+ap-northeast-2,us-west-2,0.08
+ap-southeast-1,internet,0.12
+ap-southeast-1,us-gov-east-1,0.09
+ap-southeast-1,af-south-1,0.09
+ap-southeast-1,ap-east-1,0.09
+ap-southeast-1,ap-southeast-3,0.09
+ap-southeast-1,ap-south-1,0.09
+ap-southeast-1,ap-northeast-3,0.09
+ap-southeast-1,ap-northeast-2,0.09
+ap-southeast-1,ap-southeast-2,0.09
+ap-southeast-1,ap-northeast-1,0.09
+ap-southeast-1,ca-central-1,0.09
+ap-southeast-1,eu-central-1,0.09
+ap-southeast-1,eu-west-1,0.09
+ap-southeast-1,eu-west-2,0.09
+ap-southeast-1,eu-south-1,0.09
+ap-southeast-1,eu-west-3,0.09
+ap-southeast-1,eu-south-2,0.09
+ap-southeast-1,eu-north-1,0.09
+ap-southeast-1,eu-central-2,0.09
+ap-southeast-1,me-south-1,0.09
+ap-southeast-1,me-central-1,0.09
+ap-southeast-1,sa-east-1,0.09
+ap-southeast-1,us-east-1,0.09
+ap-southeast-1,us-east-2,0.09
+ap-southeast-1,us-west-1,0.09
+ap-southeast-1,us-west-2,0.09
+ap-southeast-2,internet,0.114
+ap-southeast-2,us-gov-east-1,0.098
+ap-southeast-2,af-south-1,0.098
+ap-southeast-2,ap-east-1,0.098
+ap-southeast-2,ap-southeast-3,0.098
+ap-southeast-2,ap-south-1,0.098
+ap-southeast-2,ap-northeast-3,0.098
+ap-southeast-2,ap-northeast-2,0.098
+ap-southeast-2,ap-southeast-1,0.098
+ap-southeast-2,ap-northeast-1,0.098
+ap-southeast-2,ca-central-1,0.098
+ap-southeast-2,eu-central-1,0.098
+ap-southeast-2,eu-west-1,0.098
+ap-southeast-2,eu-west-2,0.098
+ap-southeast-2,eu-south-1,0.098
+ap-southeast-2,eu-west-3,0.098
+ap-southeast-2,eu-south-2,0.098
+ap-southeast-2,eu-north-1,0.098
+ap-southeast-2,eu-central-2,0.098
+ap-southeast-2,me-south-1,0.098
+ap-southeast-2,me-central-1,0.098
+ap-southeast-2,sa-east-1,0.098
+ap-southeast-2,us-east-1,0.098
+ap-southeast-2,us-east-2,0.098
+ap-southeast-2,us-west-1,0.098
+ap-southeast-2,us-west-2,0.098
+ap-northeast-1,internet,0.114
+ap-northeast-1,us-gov-east-1,0.09
+ap-northeast-1,af-south-1,0.09
+ap-northeast-1,ap-east-1,0.09
+ap-northeast-1,ap-southeast-3,0.09
+ap-northeast-1,ap-south-1,0.09
+ap-northeast-1,ap-northeast-3,0.09
+ap-northeast-1,ap-northeast-2,0.09
+ap-northeast-1,ap-southeast-1,0.09
+ap-northeast-1,ap-southeast-2,0.09
+ap-northeast-1,ca-central-1,0.09
+ap-northeast-1,eu-central-1,0.09
+ap-northeast-1,eu-west-1,0.09
+ap-northeast-1,eu-west-2,0.09
+ap-northeast-1,eu-south-1,0.09
+ap-northeast-1,eu-west-3,0.09
+ap-northeast-1,eu-south-2,0.09
+ap-northeast-1,eu-north-1,0.09
+ap-northeast-1,eu-central-2,0.09
+ap-northeast-1,me-south-1,0.09
+ap-northeast-1,me-central-1,0.09
+ap-northeast-1,sa-east-1,0.09
+ap-northeast-1,us-east-1,0.09
+ap-northeast-1,us-east-2,0.09
+ap-northeast-1,us-west-1,0.09
+ap-northeast-1,us-west-2,0.09
+ca-central-1,internet,0.09
+ca-central-1,us-gov-east-1,0.02
+ca-central-1,af-south-1,0.02
+ca-central-1,ap-east-1,0.02
+ca-central-1,ap-southeast-3,0.02
+ca-central-1,ap-south-1,0.02
+ca-central-1,ap-northeast-3,0.02
+ca-central-1,ap-northeast-2,0.02
+ca-central-1,ap-southeast-1,0.02
+ca-central-1,ap-southeast-2,0.02
+ca-central-1,ap-northeast-1,0.02
+ca-central-1,eu-central-1,0.02
+ca-central-1,eu-west-1,0.02
+ca-central-1,eu-west-2,0.02
+ca-central-1,eu-south-1,0.02
+ca-central-1,eu-west-3,0.02
+ca-central-1,eu-south-2,0.02
+ca-central-1,eu-north-1,0.02
+ca-central-1,eu-central-2,0.02
+ca-central-1,me-south-1,0.02
+ca-central-1,me-central-1,0.02
+ca-central-1,sa-east-1,0.02
+ca-central-1,us-east-1,0.02
+ca-central-1,us-east-2,0.02
+ca-central-1,us-west-1,0.02
+ca-central-1,us-west-2,0.02
+eu-central-1,internet,0.09
+eu-central-1,us-gov-east-1,0.02
+eu-central-1,af-south-1,0.02
+eu-central-1,ap-east-1,0.02
+eu-central-1,ap-southeast-3,0.02
+eu-central-1,ap-south-1,0.02
+eu-central-1,ap-northeast-3,0.02
+eu-central-1,ap-northeast-2,0.02
+eu-central-1,ap-southeast-1,0.02
+eu-central-1,ap-southeast-2,0.02
+eu-central-1,ap-northeast-1,0.02
+eu-central-1,ca-central-1,0.02
+eu-central-1,eu-west-1,0.02
+eu-central-1,eu-west-2,0.02
+eu-central-1,eu-south-1,0.02
+eu-central-1,eu-west-3,0.02
+eu-central-1,eu-south-2,0.02
+eu-central-1,eu-north-1,0.02
+eu-central-1,eu-central-2,0.02
+eu-central-1,me-south-1,0.02
+eu-central-1,me-central-1,0.02
+eu-central-1,sa-east-1,0.02
+eu-central-1,us-east-1,0.02
+eu-central-1,us-east-2,0.02
+eu-central-1,us-west-1,0.02
+eu-central-1,us-west-2,0.02
+eu-west-1,internet,0.09
+eu-west-1,us-gov-east-1,0.02
+eu-west-1,af-south-1,0.02
+eu-west-1,ap-east-1,0.02
+eu-west-1,ap-southeast-3,0.02
+eu-west-1,ap-south-1,0.02
+eu-west-1,ap-northeast-3,0.02
+eu-west-1,ap-northeast-2,0.02
+eu-west-1,ap-southeast-1,0.02
+eu-west-1,ap-southeast-2,0.02
+eu-west-1,ap-northeast-1,0.02
+eu-west-1,ca-central-1,0.02
+eu-west-1,eu-central-1,0.02
+eu-west-1,eu-west-2,0.02
+eu-west-1,eu-south-1,0.02
+eu-west-1,eu-west-3,0.02
+eu-west-1,eu-south-2,0.02
+eu-west-1,eu-north-1,0.02
+eu-west-1,eu-central-2,0.02
+eu-west-1,me-south-1,0.02
+eu-west-1,me-central-1,0.02
+eu-west-1,sa-east-1,0.02
+eu-west-1,us-east-1,0.02
+eu-west-1,us-east-2,0.02
+eu-west-1,us-west-1,0.02
+eu-west-1,us-west-2,0.02
+eu-west-2,internet,0.09
+eu-west-2,us-gov-east-1,0.02
+eu-west-2,af-south-1,0.02
+eu-west-2,ap-east-1,0.02
+eu-west-2,ap-southeast-3,0.02
+eu-west-2,ap-south-1,0.02
+eu-west-2,ap-northeast-3,0.02
+eu-west-2,ap-northeast-2,0.02
+eu-west-2,ap-southeast-1,0.02
+eu-west-2,ap-southeast-2,0.02
+eu-west-2,ap-northeast-1,0.02
+eu-west-2,ca-central-1,0.02
+eu-west-2,eu-central-1,0.02
+eu-west-2,eu-west-1,0.02
+eu-west-2,eu-south-1,0.02
+eu-west-2,eu-west-3,0.02
+eu-west-2,eu-south-2,0.02
+eu-west-2,eu-north-1,0.02
+eu-west-2,eu-central-2,0.02
+eu-west-2,me-south-1,0.02
+eu-west-2,me-central-1,0.02
+eu-west-2,sa-east-1,0.02
+eu-west-2,us-east-1,0.02
+eu-west-2,us-east-2,0.02
+eu-west-2,us-west-1,0.02
+eu-west-2,us-west-2,0.02
+eu-south-1,internet,0.09
+eu-south-1,us-gov-east-1,0.02
+eu-south-1,af-south-1,0.02
+eu-south-1,ap-east-1,0.02
+eu-south-1,ap-southeast-3,0.02
+eu-south-1,ap-south-1,0.02
+eu-south-1,ap-northeast-3,0.02
+eu-south-1,ap-northeast-2,0.02
+eu-south-1,ap-southeast-1,0.02
+eu-south-1,ap-southeast-2,0.02
+eu-south-1,ap-northeast-1,0.02
+eu-south-1,ca-central-1,0.02
+eu-south-1,eu-central-1,0.02
+eu-south-1,eu-west-1,0.02
+eu-south-1,eu-west-2,0.02
+eu-south-1,eu-west-3,0.02
+eu-south-1,eu-south-2,0.02
+eu-south-1,eu-north-1,0.02
+eu-south-1,eu-central-2,0.02
+eu-south-1,me-south-1,0.02
+eu-south-1,me-central-1,0.02
+eu-south-1,sa-east-1,0.02
+eu-south-1,us-east-1,0.02
+eu-south-1,us-east-2,0.02
+eu-south-1,us-west-1,0.02
+eu-south-1,us-west-2,0.02
+eu-west-3,internet,0.09
+eu-west-3,us-gov-east-1,0.02
+eu-west-3,af-south-1,0.02
+eu-west-3,ap-east-1,0.02
+eu-west-3,ap-southeast-3,0.02
+eu-west-3,ap-south-1,0.02
+eu-west-3,ap-northeast-3,0.02
+eu-west-3,ap-northeast-2,0.02
+eu-west-3,ap-southeast-1,0.02
+eu-west-3,ap-southeast-2,0.02
+eu-west-3,ap-northeast-1,0.02
+eu-west-3,ca-central-1,0.02
+eu-west-3,eu-central-1,0.02
+eu-west-3,eu-west-1,0.02
+eu-west-3,eu-west-2,0.02
+eu-west-3,eu-south-1,0.02
+eu-west-3,eu-south-2,0.02
+eu-west-3,eu-north-1,0.02
+eu-west-3,eu-central-2,0.02
+eu-west-3,me-south-1,0.02
+eu-west-3,me-central-1,0.02
+eu-west-3,sa-east-1,0.02
+eu-west-3,us-east-1,0.02
+eu-west-3,us-east-2,0.02
+eu-west-3,us-west-1,0.02
+eu-west-3,us-west-2,0.02
+eu-south-2,internet,0.09
+eu-south-2,us-gov-east-1,0.02
+eu-south-2,af-south-1,0.02
+eu-south-2,ap-east-1,0.02
+eu-south-2,ap-southeast-3,0.02
+eu-south-2,ap-south-1,0.02
+eu-south-2,ap-northeast-3,0.02
+eu-south-2,ap-northeast-2,0.02
+eu-south-2,ap-southeast-1,0.02
+eu-south-2,ap-southeast-2,0.02
+eu-south-2,ap-northeast-1,0.02
+eu-south-2,ca-central-1,0.02
+eu-south-2,eu-central-1,0.02
+eu-south-2,eu-west-1,0.02
+eu-south-2,eu-west-2,0.02
+eu-south-2,eu-south-1,0.02
+eu-south-2,eu-west-3,0.02
+eu-south-2,eu-north-1,0.02
+eu-south-2,eu-central-2,0.02
+eu-south-2,me-south-1,0.02
+eu-south-2,me-central-1,0.02
+eu-south-2,sa-east-1,0.02
+eu-south-2,us-east-1,0.02
+eu-south-2,us-east-2,0.02
+eu-south-2,us-west-1,0.02
+eu-south-2,us-west-2,0.02
+eu-north-1,internet,0.09
+eu-north-1,us-gov-east-1,0.02
+eu-north-1,af-south-1,0.02
+eu-north-1,ap-east-1,0.02
+eu-north-1,ap-southeast-3,0.02
+eu-north-1,ap-south-1,0.02
+eu-north-1,ap-northeast-3,0.02
+eu-north-1,ap-northeast-2,0.02
+eu-north-1,ap-southeast-1,0.02
+eu-north-1,ap-southeast-2,0.02
+eu-north-1,ap-northeast-1,0.02
+eu-north-1,ca-central-1,0.02
+eu-north-1,eu-central-1,0.02
+eu-north-1,eu-west-1,0.02
+eu-north-1,eu-west-2,0.02
+eu-north-1,eu-south-1,0.02
+eu-north-1,eu-west-3,0.02
+eu-north-1,eu-south-2,0.02
+eu-north-1,eu-central-2,0.02
+eu-north-1,me-south-1,0.02
+eu-north-1,me-central-1,0.02
+eu-north-1,sa-east-1,0.02
+eu-north-1,us-east-1,0.02
+eu-north-1,us-east-2,0.02
+eu-north-1,us-west-1,0.02
+eu-north-1,us-west-2,0.02
+eu-central-2,internet,0.09
+eu-central-2,us-gov-east-1,0.02
+eu-central-2,af-south-1,0.02
+eu-central-2,ap-east-1,0.02
+eu-central-2,ap-southeast-3,0.02
+eu-central-2,ap-south-1,0.02
+eu-central-2,ap-northeast-3,0.02
+eu-central-2,ap-northeast-2,0.02
+eu-central-2,ap-southeast-1,0.02
+eu-central-2,ap-southeast-2,0.02
+eu-central-2,ap-northeast-1,0.02
+eu-central-2,ca-central-1,0.02
+eu-central-2,eu-central-1,0.02
+eu-central-2,eu-west-1,0.02
+eu-central-2,eu-west-2,0.02
+eu-central-2,eu-south-1,0.02
+eu-central-2,eu-west-3,0.02
+eu-central-2,eu-south-2,0.02
+eu-central-2,eu-north-1,0.02
+eu-central-2,me-south-1,0.02
+eu-central-2,me-central-1,0.02
+eu-central-2,sa-east-1,0.02
+eu-central-2,us-east-1,0.02
+eu-central-2,us-east-2,0.02
+eu-central-2,us-west-1,0.02
+eu-central-2,us-west-2,0.02
+me-south-1,internet,0.117
+me-south-1,us-gov-east-1,0.1105
+me-south-1,af-south-1,0.1105
+me-south-1,ap-east-1,0.1105
+me-south-1,ap-southeast-3,0.1105
+me-south-1,ap-south-1,0.1105
+me-south-1,ap-northeast-3,0.1105
+me-south-1,ap-northeast-2,0.1105
+me-south-1,ap-southeast-1,0.1105
+me-south-1,ap-southeast-2,0.1105
+me-south-1,ap-northeast-1,0.1105
+me-south-1,ca-central-1,0.1105
+me-south-1,eu-central-1,0.1105
+me-south-1,eu-west-1,0.1105
+me-south-1,eu-west-2,0.1105
+me-south-1,eu-south-1,0.1105
+me-south-1,eu-west-3,0.1105
+me-south-1,eu-south-2,0.1105
+me-south-1,eu-north-1,0.1105
+me-south-1,eu-central-2,0.1105
+me-south-1,me-central-1,0.1105
+me-south-1,sa-east-1,0.1105
+me-south-1,us-east-1,0.1105
+me-south-1,us-east-2,0.1105
+me-south-1,us-west-1,0.1105
+me-south-1,us-west-2,0.1105
+me-central-1,internet,0.11
+me-central-1,us-gov-east-1,0.085
+me-central-1,af-south-1,0.085
+me-central-1,ap-east-1,0.085
+me-central-1,ap-southeast-3,0.085
+me-central-1,ap-south-1,0.085
+me-central-1,ap-northeast-3,0.085
+me-central-1,ap-northeast-2,0.085
+me-central-1,ap-southeast-1,0.085
+me-central-1,ap-southeast-2,0.085
+me-central-1,ap-northeast-1,0.085
+me-central-1,ca-central-1,0.085
+me-central-1,eu-central-1,0.085
+me-central-1,eu-west-1,0.085
+me-central-1,eu-west-2,0.085
+me-central-1,eu-south-1,0.085
+me-central-1,eu-west-3,0.085
+me-central-1,eu-south-2,0.085
+me-central-1,eu-north-1,0.085
+me-central-1,eu-central-2,0.085
+me-central-1,me-south-1,0.085
+me-central-1,sa-east-1,0.085
+me-central-1,us-east-1,0.085
+me-central-1,us-east-2,0.085
+me-central-1,us-west-1,0.085
+me-central-1,us-west-2,0.085
+sa-east-1,internet,0.15
+sa-east-1,us-gov-east-1,0.138
+sa-east-1,af-south-1,0.138
+sa-east-1,ap-east-1,0.138
+sa-east-1,ap-southeast-3,0.138
+sa-east-1,ap-south-1,0.138
+sa-east-1,ap-northeast-3,0.138
+sa-east-1,ap-northeast-2,0.138
+sa-east-1,ap-southeast-1,0.138
+sa-east-1,ap-southeast-2,0.138
+sa-east-1,ap-northeast-1,0.138
+sa-east-1,ca-central-1,0.138
+sa-east-1,eu-central-1,0.138
+sa-east-1,eu-west-1,0.138
+sa-east-1,eu-west-2,0.138
+sa-east-1,eu-south-1,0.138
+sa-east-1,eu-west-3,0.138
+sa-east-1,eu-south-2,0.138
+sa-east-1,eu-north-1,0.138
+sa-east-1,eu-central-2,0.138
+sa-east-1,me-south-1,0.138
+sa-east-1,me-central-1,0.138
+sa-east-1,us-east-1,0.138
+sa-east-1,us-east-2,0.138
+sa-east-1,us-west-1,0.138
+sa-east-1,us-west-2,0.138
+us-east-1,internet,0.09
+us-east-1,us-gov-east-1,0.02
+us-east-1,af-south-1,0.02
+us-east-1,ap-east-1,0.02
+us-east-1,ap-southeast-3,0.02
+us-east-1,ap-south-1,0.02
+us-east-1,ap-northeast-3,0.02
+us-east-1,ap-northeast-2,0.02
+us-east-1,ap-southeast-1,0.02
+us-east-1,ap-southeast-2,0.02
+us-east-1,ap-northeast-1,0.02
+us-east-1,ca-central-1,0.02
+us-east-1,eu-central-1,0.02
+us-east-1,eu-west-1,0.02
+us-east-1,eu-west-2,0.02
+us-east-1,eu-south-1,0.02
+us-east-1,eu-west-3,0.02
+us-east-1,eu-south-2,0.02
+us-east-1,eu-north-1,0.02
+us-east-1,eu-central-2,0.02
+us-east-1,me-south-1,0.02
+us-east-1,me-central-1,0.02
+us-east-1,sa-east-1,0.02
+us-east-1,us-east-2,0.01
+us-east-1,us-west-1,0.02
+us-east-1,us-west-2,0.02
+us-east-2,internet,0.09
+us-east-2,us-gov-east-1,0.02
+us-east-2,af-south-1,0.02
+us-east-2,ap-east-1,0.02
+us-east-2,ap-southeast-3,0.02
+us-east-2,ap-south-1,0.02
+us-east-2,ap-northeast-3,0.02
+us-east-2,ap-northeast-2,0.02
+us-east-2,ap-southeast-1,0.02
+us-east-2,ap-southeast-2,0.02
+us-east-2,ap-northeast-1,0.02
+us-east-2,ca-central-1,0.02
+us-east-2,eu-central-1,0.02
+us-east-2,eu-west-1,0.02
+us-east-2,eu-west-2,0.02
+us-east-2,eu-south-1,0.02
+us-east-2,eu-west-3,0.02
+us-east-2,eu-south-2,0.02
+us-east-2,eu-north-1,0.02
+us-east-2,eu-central-2,0.02
+us-east-2,me-south-1,0.02
+us-east-2,me-central-1,0.02
+us-east-2,sa-east-1,0.02
+us-east-2,us-east-1,0.01
+us-east-2,us-west-1,0.02
+us-east-2,us-west-2,0.02
+us-west-1,internet,0.09
+us-west-1,us-gov-east-1,0.02
+us-west-1,af-south-1,0.02
+us-west-1,ap-east-1,0.02
+us-west-1,ap-southeast-3,0.02
+us-west-1,ap-south-1,0.02
+us-west-1,ap-northeast-3,0.02
+us-west-1,ap-northeast-2,0.02
+us-west-1,ap-southeast-1,0.02
+us-west-1,ap-southeast-2,0.02
+us-west-1,ap-northeast-1,0.02
+us-west-1,ca-central-1,0.02
+us-west-1,eu-central-1,0.02
+us-west-1,eu-west-1,0.02
+us-west-1,eu-west-2,0.02
+us-west-1,eu-south-1,0.02
+us-west-1,eu-west-3,0.02
+us-west-1,eu-south-2,0.02
+us-west-1,eu-north-1,0.02
+us-west-1,eu-central-2,0.02
+us-west-1,me-south-1,0.02
+us-west-1,me-central-1,0.02
+us-west-1,sa-east-1,0.02
+us-west-1,us-east-1,0.02
+us-west-1,us-east-2,0.02
+us-west-1,us-west-2,0.02
+us-west-2,internet,0.09
+us-west-2,us-gov-east-1,0.02
+us-west-2,af-south-1,0.02
+us-west-2,ap-east-1,0.02
+us-west-2,ap-southeast-3,0.02
+us-west-2,ap-south-1,0.02
+us-west-2,ap-northeast-3,0.02
+us-west-2,ap-northeast-2,0.02
+us-west-2,ap-southeast-1,0.02
+us-west-2,ap-southeast-2,0.02
+us-west-2,ap-northeast-1,0.02
+us-west-2,ca-central-1,0.02
+us-west-2,eu-central-1,0.02
+us-west-2,eu-west-1,0.02
+us-west-2,eu-west-2,0.02
+us-west-2,eu-south-1,0.02
+us-west-2,eu-west-3,0.02
+us-west-2,eu-south-2,0.02
+us-west-2,eu-north-1,0.02
+us-west-2,eu-central-2,0.02
+us-west-2,me-south-1,0.02
+us-west-2,me-central-1,0.02
+us-west-2,sa-east-1,0.02
+us-west-2,us-east-1,0.02
+us-west-2,us-east-2,0.02
+us-west-2,us-west-1,0.02
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/exceptions.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,20 @@
     def pretty_print_str(self):
         err = f"[red][bold]:x: InsufficientVCPUException:[/bold] {str(self)}[/red]"
         err += "\n[bold][red]Please ensure that you have enough vCPUs in the given region.[/red][/bold]"
         # todo print link to a documentation page to request more vCPUs
         return err
 
 
+class GatewayContainerStartException(SkyplaneException):
+    def pretty_print_str(self):
+        err = f"[red][bold]:x: GatewayContainerStartException:[/bold] {str(self)}[/red]"
+        return err
+
+
 class TransferFailedException(SkyplaneException):
     def __init__(self, message, failed_objects=None):
         super().__init__(message)
         self.failed_objects = failed_objects
 
     def pretty_print_str(self):
         err = f"[red][bold]:x: TransferFailedException:[/bold] {str(self)}[/red]"
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/azure_storage_account_interface.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/azure_storage_account_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class AzureStorageAccountInterface:
     """Class to manage state for an Azure storage account. Note that storage account names are globally unique."""
 
     def __init__(self, account_name: str):
         self.auth = compute.AzureAuthentication()
         self.account_name = account_name
+        self.provider = "azure"
 
     @lru_cache(maxsize=1)
     def storage_account_obj(self):
         sm_client = self.auth.get_storage_management_client()
         storage_accounts = sm_client.storage_accounts.list()
         for storage_account in storage_accounts:
             if storage_account.name == self.account_name:
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/gcs_interface.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/gcs_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 import datetime
 import hashlib
 import os
 from functools import lru_cache
 from xml.etree import ElementTree
 
 import requests
-from typing import Iterator, List, Optional, Tuple
+from typing import Any, Iterator, List, Optional, Tuple
 
 from skyplane import exceptions, compute
 from skyplane.config_paths import cloud_config
 from skyplane.exceptions import NoSuchObjectException
 from skyplane.obj_store.object_store_interface import ObjectStoreInterface, ObjectStoreObject
 from skyplane.utils import logger
+from skyplane.utils.generator import batch_generator
 
 
 class GCSObject(ObjectStoreObject):
     def full_path(self):
         return os.path.join(f"gs://{self.bucket}", self.key)
 
 
 class GCSInterface(ObjectStoreInterface):
     def __init__(self, bucket_name: str):
         self.bucket_name = bucket_name
         self.auth = compute.GCPAuthentication()
         self._gcs_client = self.auth.get_storage_client()
         self._requests_session = requests.Session()
 
+    @property
+    def provider(self):
+        return "gcp"
+
     def path(self):
         return f"gs://{self.bucket_name}"
 
     @property
     @lru_cache(maxsize=1)
     def gcp_region(self):
         def map_region_to_zone(region) -> str:
@@ -96,20 +101,30 @@
         if not self.bucket_exists():
             bucket = self._gcs_client.bucket(self.bucket_name)
             bucket.storage_class = "STANDARD"
             region_without_zone = "-".join(gcp_region.split("-")[:2])
             self._gcs_client.create_bucket(bucket, location=region_without_zone)
 
     def delete_bucket(self):
+        for batch in batch_generator(self.list_objects(), 1000):
+            self.delete_objects([obj.key for obj in batch])
+        assert len(list(self.list_objects())) == 0, f"Bucket not empty after deleting all keys {list(self.list_objects())}"
         self._gcs_client.get_bucket(self.bucket_name).delete()
 
-    def list_objects(self, prefix="") -> Iterator[GCSObject]:
+    def list_objects(self, prefix="", region=None) -> Iterator[GCSObject]:
         blobs = self._gcs_client.list_blobs(self.bucket_name, prefix=prefix)
         for blob in blobs:
-            yield GCSObject("gcs", self.bucket_name, blob.name, blob.size, blob.updated, mime_type=getattr(blob, "content_type", None))
+            yield GCSObject(
+                blob.name,
+                provider="gcp",
+                bucket=self.bucket_name,
+                size=blob.size,
+                last_modified=blob.updated,
+                mime_type=getattr(blob, "content_type", None),
+            )
 
     def delete_objects(self, keys: List[str]):
         for key in keys:
             self._gcs_client.bucket(self.bucket_name).blob(key).delete()
 
     @lru_cache(maxsize=1024)
     def get_obj_metadata(self, obj_name):
@@ -210,38 +225,42 @@
                     raise exceptions.ChecksumMismatchException(
                         f"Checksum mismatch for object {dst_object_name} in bucket {self.bucket_name}, "
                         + f"expected {b64_md5sum}, got {blob_md5}"
                     )
             return
 
         # multipart upload
-        assert part_number is not None and upload_id is not None
+        assert part_number is not None, f"Part number cannot be none for multipart upload: {part_number}, {upload_id}"
+        assert upload_id is not None, f"Upload ID cannot be none for multipart upload: {part_number}, {upload_id}"
 
         # send XML api request
         headers = {"Content-MD5": b64_md5sum} if check_md5 else None
-        response = self.send_xml_request(
-            dst_object_name,
-            {"uploadId": upload_id, "partNumber": part_number},
-            "PUT",
-            headers=headers,
-            data=open(src_file_path, "rb"),
-        )
+        try:
+            response = self.send_xml_request(
+                dst_object_name,
+                {"uploadId": upload_id, "partNumber": part_number},
+                "PUT",
+                headers=headers,
+                data=open(src_file_path, "rb"),
+            )
+        except Exception as e:
+            raise ValueError(f"Failed to upload {dst_object_name} to bucket {self.bucket_name} upload id {upload_id}: {e}")
 
         # check response
         if "ETag" not in response.headers:
             raise exceptions.ChecksumMismatchException(
                 f"Upload of object {dst_object_name} in bucket {self.bucket_name} failed, got status code {response.status_code} w/ response {response.text}"
             )
 
     def initiate_multipart_upload(self, dst_object_name: str, mime_type: Optional[str] = None) -> str:
         assert len(dst_object_name) > 0, f"Destination object name must be non-empty: '{dst_object_name}'"
         response = self.send_xml_request(dst_object_name, {"uploads": None}, "POST", content_type=mime_type)
         return ElementTree.fromstring(response.content)[2].text
 
-    def complete_multipart_upload(self, dst_object_name, upload_id):
+    def complete_multipart_upload(self, dst_object_name, upload_id, metadata: Optional[Any] = None):
         # get parts
         xml_data = ElementTree.Element("CompleteMultipartUpload")
         next_part_number_marker = None
 
         # Parts in the list are ordered sequentially, and the XML API does not return lists longer than 1000 parts.
         while True:
             if next_part_number_marker is None:
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/object_store_interface.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/object_store_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,38 @@
 from dataclasses import dataclass
 
-from typing import Iterator, List, Optional, Tuple
+from typing import Any, Iterator, List, Optional, Tuple
+
+from skyplane.obj_store.storage_interface import StorageInterface
+from skyplane.utils import logger
 
 
 @dataclass
 class ObjectStoreObject:
     """Defines object in object store."""
 
-    provider: str
-    bucket: str
     key: str
+    provider: Optional[str] = None
+    bucket: Optional[str] = None
     size: Optional[int] = None
     last_modified: Optional[str] = None
     mime_type: Optional[str] = None
 
     @property
     def exists(self):
         return self.size is not None and self.last_modified is not None
 
     def full_path(self):
         raise NotImplementedError()
 
 
-class ObjectStoreInterface:
-    def path(self) -> str:
-        raise NotImplementedError()
-
-    def region_tag(self) -> str:
-        raise NotImplementedError()
-
-    def bucket(self) -> str:
-        raise NotImplementedError()
-
+class ObjectStoreInterface(StorageInterface):
     def set_requester_bool(self, requester: bool):
         return
 
-    def create_bucket(self, region_tag: str):
-        raise NotImplementedError()
-
-    def delete_bucket(self):
-        raise NotImplementedError()
-
-    def bucket_exists(self) -> bool:
-        raise NotImplementedError()
-
-    def exists(self, obj_name: str) -> bool:
-        raise NotImplementedError()
-
-    def list_objects(self, prefix="") -> Iterator[ObjectStoreObject]:
-        raise NotImplementedError()
-
     def get_obj_size(self, obj_name) -> int:
         raise NotImplementedError()
 
     def get_obj_last_modified(self, obj_name):
         raise NotImplementedError()
 
     def get_obj_mime_type(self, obj_name):
@@ -99,27 +78,9 @@
 
     def delete_objects(self, keys: List[str]):
         raise NotImplementedError()
 
     def initiate_multipart_upload(self, dst_object_name: str, mime_type: Optional[str] = None) -> str:
         raise ValueError("Multipart uploads not supported")
 
-    def complete_multipart_upload(self, dst_object_name: str, upload_id: str) -> None:
+    def complete_multipart_upload(self, dst_object_name: str, upload_id: str, metadata: Optional[Any] = None) -> None:
         raise ValueError("Multipart uploads not supported")
-
-    @staticmethod
-    def create(region_tag: str, bucket: str):
-        if region_tag.startswith("aws"):
-            from skyplane.obj_store.s3_interface import S3Interface
-
-            return S3Interface(bucket)
-        elif region_tag.startswith("gcp"):
-            from skyplane.obj_store.gcs_interface import GCSInterface
-
-            return GCSInterface(bucket)
-        elif region_tag.startswith("azure"):
-            from skyplane.obj_store.azure_blob_interface import AzureBlobInterface
-
-            storage_account, container = bucket.split("/", 1)  # <storage_account>/<container>
-            return AzureBlobInterface(storage_account, container)
-        else:
-            raise ValueError(f"Invalid region_tag {region_tag} - could not create interface")
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/obj_store/s3_interface.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/obj_store/s3_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import base64
 import hashlib
 import os
 from functools import lru_cache
 
-from typing import Iterator, List, Optional, Tuple
+from typing import Any, Iterator, List, Optional, Tuple
 
 from skyplane import exceptions, compute
 from skyplane.exceptions import NoSuchObjectException
 from skyplane.obj_store.object_store_interface import ObjectStoreInterface, ObjectStoreObject
 from skyplane.config_paths import cloud_config
 from skyplane.utils import logger, imports
+from skyplane.utils.generator import batch_generator
 
 
 class S3Object(ObjectStoreObject):
     def full_path(self):
         return f"s3://{self.bucket}/{self.key}"
 
 
 class S3Interface(ObjectStoreInterface):
     def __init__(self, bucket_name: str):
         self.auth = compute.AWSAuthentication()
         self.requester_pays = False
         self.bucket_name = bucket_name
         self._cached_s3_clients = {}
 
+    @property
+    def provider(self):
+        return "aws"
+
     def path(self):
         return f"s3://{self.bucket_name}"
 
     @property
     @lru_cache(maxsize=1)
     def aws_region(self):
         s3_client = self.auth.get_boto3_client("s3")
@@ -36,16 +41,20 @@
             # None means us-east-1 for legacy reasons
             region = s3_client.get_bucket_location(Bucket=self.bucket_name).get("LocationConstraint", "us-east-1")
             return region if region is not None else default_region
         except Exception as e:
             if "An error occurred (AccessDenied) when calling the GetBucketLocation operation" in str(e):
                 logger.warning(f"Bucket location {self.bucket_name} is not public. Assuming region is {default_region}")
                 return default_region
-            logger.warning(f"Specified bucket {self.bucket_name} does not exist, got AWS error: {e}")
-            raise exceptions.MissingBucketException(f"S3 bucket {self.bucket_name} does not exist") from e
+            elif "An error occurred (InvalidAccessKeyId) when calling" in str(e):
+                logger.warning(f"Invalid AWS credentials. Check to make sure credentials configured properly.")
+                raise exceptions.PermissionsException(f"Invalid AWS credentials for accessing bucket {self.bucket_name}")
+            else:
+                logger.warning(f"Specified bucket {self.bucket_name} does not exist, got AWS error: {e}")
+                raise exceptions.MissingBucketException(f"S3 bucket {self.bucket_name} does not exist") from e
 
     def region_tag(self):
         return "aws:" + self.aws_region
 
     def bucket(self) -> str:
         return self.bucket_name
 
@@ -55,45 +64,65 @@
     def _s3_client(self, region=None):
         region = region if region is not None else self.aws_region
         if region not in self._cached_s3_clients:
             self._cached_s3_clients[region] = self.auth.get_boto3_client("s3", region)
         return self._cached_s3_clients[region]
 
     @imports.inject("botocore.exceptions", pip_extra="aws")
-    def bucket_exists(botocore_exceptions, self):
-        s3_client = self._s3_client("us-east-1")
+    def bucket_exists(botocore_exceptions, self, region=None):
+        if region is None:  # use current bucket region is available
+            try:
+                region = self.aws_region
+            except exceptions.MissingBucketException:
+                region = "us-east-1"
+
+        s3_client = self._s3_client(region)
         try:
             requester_pays = {"RequestPayer": "requester"} if self.requester_pays else {}
             s3_client.list_objects_v2(Bucket=self.bucket_name, MaxKeys=1, **requester_pays)
             return True
         except botocore_exceptions.ClientError as e:
             if e.response["Error"]["Code"] == "NoSuchBucket" or e.response["Error"]["Code"] == "AccessDenied":
                 return False
             raise
 
     def create_bucket(self, aws_region):
         s3_client = self._s3_client(aws_region)
-        if not self.bucket_exists():
+        if not self.bucket_exists(aws_region):
             if aws_region == "us-east-1":
                 s3_client.create_bucket(Bucket=self.bucket_name)
             else:
                 s3_client.create_bucket(Bucket=self.bucket_name, CreateBucketConfiguration={"LocationConstraint": aws_region})
+        else:
+            logger.warning(f"Bucket {self.bucket} in region {aws_region} already exists")
 
     def delete_bucket(self):
+        # delete 1000 keys at a time
+        for batch in batch_generator(self.list_objects(), 1000):
+            self.delete_objects([obj.key for obj in batch])
+        assert len(list(self.list_objects())) == 0, f"Bucket not empty after deleting all keys {list(self.list_objects())}"
+        # delete bucket
         self._s3_client().delete_bucket(Bucket=self.bucket_name)
 
-    def list_objects(self, prefix="") -> Iterator[S3Object]:
-        paginator = self._s3_client().get_paginator("list_objects_v2")
+    def list_objects(self, prefix="", region=None) -> Iterator[S3Object]:
+        paginator = self._s3_client(region).get_paginator("list_objects_v2")
         requester_pays = {"RequestPayer": "requester"} if self.requester_pays else {}
         page_iterator = paginator.paginate(Bucket=self.bucket_name, Prefix=prefix, **requester_pays)
         for page in page_iterator:
             objs = []
             for obj in page.get("Contents", []):
                 objs.append(
-                    S3Object("aws", self.bucket_name, obj["Key"], obj["Size"], obj["LastModified"], mime_type=obj.get("ContentType"))
+                    S3Object(
+                        obj["Key"],
+                        provider=self.provider,
+                        bucket=self.bucket(),
+                        size=obj["Size"],
+                        last_modified=obj["LastModified"],
+                        mime_type=obj.get("ContentType"),
+                    )
                 )
             yield from objs
 
     def delete_objects(self, keys: List[str]):
         s3_client = self._s3_client()
         while keys:
             batch, keys = keys[:1000], keys[1000:]  # take up to 1000 keys at a time
@@ -201,15 +230,15 @@
             Bucket=self.bucket_name, Key=dst_object_name, **(dict(ContentType=mime_type) if mime_type else dict())
         )
         if "UploadId" in response:
             return response["UploadId"]
         else:
             raise exceptions.SkyplaneException(f"Failed to initiate multipart upload for {dst_object_name}: {response}")
 
-    def complete_multipart_upload(self, dst_object_name, upload_id):
+    def complete_multipart_upload(self, dst_object_name, upload_id, metadata: Optional[Any] = None):
         s3_client = self._s3_client()
         all_parts = []
         while True:
             response = s3_client.list_parts(
                 Bucket=self.bucket_name, Key=dst_object_name, MaxParts=100, UploadId=upload_id, PartNumberMarker=len(all_parts)
             )
             if "Parts" not in response:
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/planner/solver.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/planner/solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 from typing import Dict, List, Optional, Tuple
 
 from skyplane import compute
-from skyplane.planner.topology import ReplicationTopology
+from skyplane.planner.topology import TopologyPlan
 from skyplane.utils import logger
 from skyplane.utils.definitions import GB
 
 GBIT_PER_GBYTE = 8
 
 
 @dataclass
@@ -227,15 +227,15 @@
                     label = f"{solution.var_edge_flow_gigabits[i, j]:.2f} Gbps (of {solution.problem.const_throughput_grid_gbits[i, j]:.2f}Gbps), "
                     label += f"\n${link_cost:.4f}/GB over {solution.var_conn[i, j]:.1f}c"
                     src_label = f"{src.replace(':', '/')}x{solution.var_instances_per_region[i]:.1f}"
                     dst_label = f"{dst.replace(':', '/')}x{solution.var_instances_per_region[j]:.1f}"
                     g.edge(src_label, dst_label, label=label)
         return g
 
-    def to_replication_topology(self, solution: ThroughputSolution, scale_to_capacity=True) -> Tuple[ReplicationTopology, float]:
+    def to_replication_topology(self, solution: ThroughputSolution, scale_to_capacity=True) -> Tuple[TopologyPlan, float]:
         regions = self.get_regions()
         Edge = namedtuple("Edge", ["src_region", "src_instance_idx", "dst_region", "dst_instance_idx", "connections"])
 
         # check is feasible
         if not solution.is_feasible:
             raise ValueError("Solution is not feasible")
 
@@ -316,17 +316,17 @@
             bottleneck_capacity = max(list(conns_egress.values()) + list(conns_ingress.values()))
             scale_factor = 64 / bottleneck_capacity
             logger.fs.warning(f"Scaling connections by {scale_factor:.2f}x")
             dst_edges = [e._replace(connections=int(e.connections * scale_factor)) for e in dst_edges]
         else:
             scale_factor = 1.0
 
-        # build ReplicationTopology
+        # build TopologyPlan
         obj_store_edges = set()
-        replication_topology = ReplicationTopology()
+        replication_topology = TopologyPlan(src_region_tag=e.src_region, dest_region_tags=[e.dst_region])
         for e in dst_edges:
             if e.connections >= 1:
                 # connect source to destination
                 replication_topology.add_instance_instance_edge(
                     src_region=e.src_region,
                     src_instance=e.src_instance_idx,
                     dest_region=e.dst_region,
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/planner/solver_ilp.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/planner/solver_ilp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import cvxpy as cp  # type: ignore
 
 from skyplane.planner.solver import ThroughputSolver, ThroughputProblem, GBIT_PER_GBYTE, ThroughputSolution
-from skyplane.utils import logger
 
 
 class ThroughputSolverILP(ThroughputSolver):
     @staticmethod
     def choose_solver():
         installed = cp.installed_solvers()
         order = ["GUROBI", "CBC", "GLPK_MI"]
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/planner/solver_ron.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/planner/solver_ron.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/cache.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/cache.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/definitions.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/fn.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if n == -1:
         n = len(args_list)
 
     def wrapped_fn(args):
         try:
             return args, func(args)
         except Exception as e:
-            logger.error(f"Error running {func.__name__}: {e}")
+            logger.error(f"Error running {func.__name__}, {args}: {e}")
             raise
 
     results = []
     with Progress(
         SpinnerColumn(), TextColumn(desc), BarColumn(), MofNCompleteColumn(), TimeElapsedColumn(), disable=not spinner, transient=True
     ) as progress:
         progress_task = progress.add_task("", total=len(args_list))
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/imports.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def wrapper(fn):
         @functools.wraps(fn)
         def wrapped(*args, **kwargs):
             modules_imported = []
             for module in modules:
                 err_msg = f"Cannot import {module}."
                 if pip_extra:
-                    err_msg += f" Install skyplane with {pip_extra} support: `pip install skyplane[{pip_extra.lower()}]`"
+                    err_msg += f" Install skyplane with {pip_extra} support: `pip install 'skyplane[{pip_extra.lower()}]'`"
                 try:
                     modules_imported.append(importlib.import_module(module))
                 except ImportError as e:
                     module_split = module.split(".")
                     if len(module_split) > 1:  # try the "from x import y" syntax
                         try:
                             module_imported = importlib.import_module(".".join(module_split[:-1]))
```

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/logger.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/logger.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/retry.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/retry.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/skyplane/utils/timer.py` & `skyplane_nightly-0.3.2.dev20230622/skyplane/utils/timer.py`

 * *Files identical despite different names*

### Comparing `skyplane-nightly-0.2.1.dev20230312/PKG-INFO` & `skyplane_nightly-0.3.2.dev20230622/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 Metadata-Version: 2.1
 Name: skyplane-nightly
-Version: 0.2.1.dev20230312
+Version: 0.3.2.dev20230622
 Summary: Skyplane efficiently transports data between cloud regions and providers.
 Home-page: https://skyplane.org/
 License: Apache-2.0
 Author: Skyplane authors
 Author-email: skyplaneproject@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: gateway
 Provides-Extra: gcp
+Provides-Extra: ibm
 Provides-Extra: solver
-Requires-Dist: azure-identity (>=1.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-mgmt-authorization (>=1.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-mgmt-compute (>=24.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-mgmt-network (>=10.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-mgmt-resource (>=11.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-mgmt-storage (>=11.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-mgmt-subscription (>=1.0.0); extra == "azure" or extra == "all"
-Requires-Dist: azure-storage-blob (>=12.0.0); extra == "azure" or extra == "all"
-Requires-Dist: boto3 (>=1.16.0); extra == "aws" or extra == "all"
+Requires-Dist: azure-identity (>=1.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-mgmt-authorization (>=1.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-mgmt-compute (>=24.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-mgmt-network (>=10.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-mgmt-quota (>=1.1.0b3) ; extra == "azure"
+Requires-Dist: azure-mgmt-resource (>=11.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-mgmt-storage (>=11.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-mgmt-subscription (>=1.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-storage-blob (>=12.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: boto3 (>=1.16.0) ; extra == "aws" or extra == "all"
 Requires-Dist: cachetools (>=4.1.0)
 Requires-Dist: cryptography (>=1.4.0)
-Requires-Dist: cvxpy[cvxopt] (>=1.1.0); extra == "solver"
-Requires-Dist: flask (>=2.1.2,<3.0.0); extra == "gateway"
-Requires-Dist: google-api-python-client (>=2.0.2); extra == "gcp" or extra == "all"
-Requires-Dist: google-auth (>=2.0.0); extra == "gcp" or extra == "all"
-Requires-Dist: google-cloud-compute (>=1.0.0); extra == "gcp" or extra == "all"
-Requires-Dist: google-cloud-storage (>=1.30.0); extra == "gcp" or extra == "all"
-Requires-Dist: graphviz (>=0.15); extra == "solver"
-Requires-Dist: lz4 (>=4.0.0,<5.0.0); extra == "gateway"
-Requires-Dist: matplotlib (>=3.0.0); extra == "solver"
-Requires-Dist: numpy (>=1.19.0); extra == "solver"
+Requires-Dist: cvxpy (>=1.1.0) ; extra == "solver"
+Requires-Dist: flask (>=2.1.2,<3.0.0) ; extra == "gateway"
+Requires-Dist: google-api-python-client (>=2.0.2) ; extra == "gcp" or extra == "all"
+Requires-Dist: google-auth (>=2.0.0) ; extra == "gcp" or extra == "all"
+Requires-Dist: google-cloud-compute (>=1.0.0) ; extra == "gcp" or extra == "all"
+Requires-Dist: google-cloud-dataproc (>=5.4.0,<6.0.0)
+Requires-Dist: google-cloud-storage (>=1.30.0) ; extra == "gcp" or extra == "all"
+Requires-Dist: graphviz (>=0.15) ; extra == "solver"
+Requires-Dist: ibm-cloud-sdk-core (>=3.16.2) ; extra == "ibm" or extra == "all"
+Requires-Dist: ibm-cos-sdk (>=2.12.2) ; extra == "ibm" or extra == "all"
+Requires-Dist: ibm-cos-sdk-core (>=2.12.2)
+Requires-Dist: ibm-cos-sdk-s3transfer (>=2.12.2)
+Requires-Dist: ibm-vpc (>=0.15.0) ; extra == "ibm" or extra == "all"
+Requires-Dist: lz4 (>=4.0.0,<5.0.0) ; extra == "gateway"
+Requires-Dist: matplotlib (>=3.0.0) ; extra == "solver"
+Requires-Dist: numpy (>=1.19.0) ; extra == "solver"
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: paramiko (>=2.7.2)
-Requires-Dist: pynacl (>=1.5.0,<2.0.0); extra == "gateway"
-Requires-Dist: pyopenssl (>=22.0.0,<23.0.0); extra == "gateway"
+Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
+Requires-Dist: pynacl (>=1.5.0,<2.0.0) ; extra == "gateway"
+Requires-Dist: pyopenssl (>=22.0.0,<23.0.0) ; extra == "gateway"
 Requires-Dist: questionary (>=1.8.0)
 Requires-Dist: requests (>=2.23.0)
 Requires-Dist: rich (>=9.0.0)
 Requires-Dist: sshtunnel (>=0.3.0)
 Requires-Dist: typer (>=0.4.0)
-Requires-Dist: werkzeug (>=2.1.2,<3.0.0); extra == "gateway"
+Requires-Dist: werkzeug (>=2.1.2,<3.0.0) ; extra == "gateway"
 Project-URL: Documentation, https://skyplane.org/
 Project-URL: Repository, https://github.com/skyplane-project/skyplane
 Description-Content-Type: text/markdown
 
 <picture>
     <source srcset="docs/_static/logo-dark-mode.png" media="(prefers-color-scheme: dark)">
     <img src="docs/_static/logo-light-mode.png" width="300" />
@@ -66,28 +76,29 @@
 **🔥 Blazing fast bulk data transfers between any cloud 🔥**
 
 Skyplane is a tool for blazingly fast bulk data transfers between object stores in the cloud. It provisions a fleet of VMs in the cloud to transfer data in parallel while using compression and bandwidth tiering to reduce cost.
 
 Skyplane is:
 1. 🔥 Blazing fast ([110x faster than AWS DataSync](https://skyplane.org/en/latest/benchmark.html))
 2. 🤑 Cheap (4x cheaper than rsync)
-3. 🌐 Universal (AWS, Azure and GCP)
+3. 🌐 Universal (AWS, Azure, IBM and GCP)
 
 You can use Skyplane to transfer data: 
 * between object stores within a cloud provider (e.g. AWS us-east-1 to AWS us-west-2)
 * between object stores across multiple cloud providers (e.g. AWS us-east-1 to GCP us-central1)
 * between local storage and cloud object stores (experimental)
 
 Skyplane currently supports the following source and destination endpoints (any source and destination can be combined): 
 
 | Endpoint           | Source             | Destination        |
 |--------------------|--------------------|--------------------|
 | AWS S3             | :white_check_mark: | :white_check_mark: |
 | Google Storage     | :white_check_mark: | :white_check_mark: |
 | Azure Blob Storage | :white_check_mark: | :white_check_mark: |
+| IBM Cloud Object Storage | :white_check_mark: | :white_check_mark: |
 | Local Disk         | :white_check_mark: | (in progress)      |
 
 Skyplane is an actively developed project. It will have 🔪 SHARP EDGES 🔪. Please file an issue or ask the contributors via [the #help channel on our Slack](https://join.slack.com/t/skyplaneworkspace/shared_invite/zt-1cxmedcuc-GwIXLGyHTyOYELq7KoOl6Q) if you encounter bugs.
 
 # Resources 
 - [Quickstart](#quickstart)
 - [Contributing](https://skyplane.org/en/latest/contributing.html)
@@ -98,20 +109,22 @@
 
 ## 1. Installation
 We recommend installation from PyPi:
 ```
 $ pip install "skyplane[aws]"
 
 # install support for other clouds as needed:
+
 #   $ pip install "skyplane[azure]"
 #   $ pip install "skyplane[gcp]"
+#   $ pip install "skyplane[ibmcloud]"
 #   $ pip install "skyplane[all]"
 ```
 
-Skyplane supports AWS, Azure, and GCP. You can install Skyplane with support for one or more of these clouds by specifying the corresponding extras. To install two out of three clouds, you can run `pip install "skyplane[aws,azure]"`.
+Skyplane supports AWS, Azure, IBM and GCP. You can install Skyplane with support for one or more of these clouds by specifying the corresponding extras. To install two out of three clouds, you can run `pip install "skyplane[aws,azure]"`.
 
 *GCP support on the M1 Mac*: If you are using an M1 Mac with the arm64 architecture and want to install GCP support for Skyplane, you will need to install as follows
 `GRPC_PYTHON_BUILD_SYSTEM_OPENSSL=1 GRPC_PYTHON_BUILD_SYSTEM_ZLIB=1 pip install "skyplane[aws,gcp]"`
 
 ## 2. Setup Cloud Credentials 
 
 Skyplane needs access to cloud credentials to perform transfers. To get started with setting up credentials, make sure you have cloud provider CLI tools installed:
@@ -121,25 +134,34 @@
 $ pip install awscli
 
 ---> For Google Cloud:
 $ pip install gcloud
 
 ---> For Azure:
 $ pip install azure
+
 ```
 Once you have the CLI tools setup, log into each cloud provider's CLI:
 ```
 ---> For AWS:
 $ aws configure
 
 ---> For Google Cloud:
 $ gcloud auth application-default login
 
 ---> For Azure:
 $ az login
+
+---> For IBM Cloud:
+$ Follow IBM Cloud and create an account with the resource group.
+Copy https://github.com/skyplane-project/skyplane/blob/main/skyplane/compute/ibmcloud/ibm_credentials.yaml.template
+into `~/.bluemix/ibm_credentials` and fill your 
+IBM IAM key and credentials to your IBM Cloud object storage 
+
+
 ```
 After authenticating with each cloud provider, you can run `skyplane init` to create a configuration file for Skyplane.
 
 ```bash
 $ skyplane init
 ```
 <details>
```

