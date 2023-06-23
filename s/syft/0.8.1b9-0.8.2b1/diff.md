# Comparing `tmp/syft-0.8.1b9.tar.gz` & `tmp/syft-0.8.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b9.tar", last modified: Tue Jun 13 12:39:01 2023, max compression
+gzip compressed data, was "syft-0.8.2b1.tar", last modified: Fri Jun 23 12:24:03 2023, max compression
```

## Comparing `syft-0.8.1b9.tar` & `syft-0.8.2b1.tar`

### file list

```diff
@@ -1,194 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.568848 syft-0.8.1b9/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-13 12:36:14.000000 syft-0.8.1b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 12:36:14.000000 syft-0.8.1b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-13 12:39:01.568848 syft-0.8.1b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-13 12:36:13.000000 syft-0.8.1b9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 12:36:14.000000 syft-0.8.1b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-13 12:39:01.568848 syft-0.8.1b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 12:36:14.000000 syft-0.8.1b9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.544848 syft-0.8.1b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.548848 syft-0.8.1b9/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-13 12:36:31.000000 syft-0.8.1b9/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-13 12:36:31.000000 syft-0.8.1b9/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.548848 syft-0.8.1b9/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.552848 syft-0.8.1b9/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24709 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.552848 syft-0.8.1b9/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.552848 syft-0.8.1b9/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.552848 syft-0.8.1b9/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.556848 syft-0.8.1b9/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.556848 syft-0.8.1b9/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.556848 syft-0.8.1b9/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    48110 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22321 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21667 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46382 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.560848 syft-0.8.1b9/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.564848 syft-0.8.1b9/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20654 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.564848 syft-0.8.1b9/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.564848 syft-0.8.1b9/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.564848 syft-0.8.1b9/src/syft/service/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.564848 syft-0.8.1b9/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.568848 syft-0.8.1b9/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.568848 syft-0.8.1b9/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-13 12:36:14.000000 syft-0.8.1b9/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:39:01.548848 syft-0.8.1b9/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 12:39:01.000000 syft-0.8.1b9/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.636549 syft-0.8.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-23 12:20:59.000000 syft-0.8.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 12:20:59.000000 syft-0.8.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-06-23 12:24:03.636549 syft-0.8.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16170 2023-06-23 12:20:59.000000 syft-0.8.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 12:20:59.000000 syft-0.8.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-23 12:24:03.640550 syft-0.8.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 12:20:59.000000 syft-0.8.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.616549 syft-0.8.2b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.620549 syft-0.8.2b1/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 12:21:12.000000 syft-0.8.2b1/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-23 12:21:12.000000 syft-0.8.2b1/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.620549 syft-0.8.2b1/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.624549 syft-0.8.2b1/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.624549 syft-0.8.2b1/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.624549 syft-0.8.2b1/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.624549 syft-0.8.2b1/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25535 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41764 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.624549 syft-0.8.2b1/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.628549 syft-0.8.2b1/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.628549 syft-0.8.2b1/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.628549 syft-0.8.2b1/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:20:59.000000 syft-0.8.2b1/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48704 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.628549 syft-0.8.2b1/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24725 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.628549 syft-0.8.2b1/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.628549 syft-0.8.2b1/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48081 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26287 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.632549 syft-0.8.2b1/src/syft/service/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.636549 syft-0.8.2b1/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.636549 syft-0.8.2b1/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25848 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.636549 syft-0.8.2b1/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.636549 syft-0.8.2b1/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    27090 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22738 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-23 12:21:00.000000 syft-0.8.2b1/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:24:03.620549 syft-0.8.2b1/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 12:24:03.000000 syft-0.8.2b1/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b9/LICENSE` & `syft-0.8.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/PKG-INFO` & `syft-0.8.2b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,134 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b9
+Version: 0.8.2b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: dev
+Provides-Extra: telemetry
 Provides-Extra: test_plugins
 Provides-Extra: oblv
 License-File: LICENSE
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
-Perform `numpy`-like analysis on `data` that remains in `someone else's` server
+Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
+✅ `Linux` ✅ `macOS` ✅ `Windows`\* ✅ `Docker` ✅ `Kubernetes`
 
-## Install syft on Python 3.9 - 3.11
+## Install Client
 
 ```bash
 $ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
-## Launch a python dev Domain
+## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8,<0.8.1")
+sy.requires(">=0.8.1,<0.8.2")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
-## Connect with our Python Client
+## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8,<0.8.1")
+sy.requires(">=0.8.1,<0.8.2")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
+## PySyft in 10 minutes
+
+📝 <a href="/notebooks/api">API Example Notebooks</a>
+
+- <a href="/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+
+## Deploy Kubernetes Helm Chart
+
+```
+$ kubectl create namespace syft
+$ helm install my-domain syft --namespace syft --version 0.8.1 --repo https://openmined.github.io/PySyft/helm
+```
+
+### Azure or GCP Ingress
+
+```
+$ helm install ... --set ingress.ingressClass="azure/application-gateway"
+$ helm install ... --set ingress.ingressClass="gce"
+```
+
 ## Deploy to a Container Engine or Cloud
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
+1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
    `pip install -U hagrid`
 
 2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
    `hagrid quickstart`
 
 3. In the tutorial you will learn how to install and deploy:  
    `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
 
    `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
-4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
-
 ## Docs and Support
 
-- 📝 <a href="/notebooks/api">API Example Notebooks</a>
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
-  †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
-  \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
-  ‡`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
-- PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
+- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
+- PySyft 0.8.1 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
+  \*`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
+- PyGrid Requires: 🐳 `docker`, ☸️ `kubernetes` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
-`0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
+`0.9.0` - Coming soon...  
+`0.8.2` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.1` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
@@ -126,14 +151,15 @@
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
 No more cold calls to get `access` to a dataset. No more weeks of `wait times` to get a `result` on your `query`. It also means `1000x more data` in every domain. PySyft opens the doors to a streamlined Data Scientist `workflow`, all with the individual's `privacy` at its heart.
 
+<!--
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
@@ -182,14 +208,15 @@
 - Deploy to GCP
 - Deploy to Kubernetes
 - Customize Networking
 - Modify PyGrid UI
 </td>
 </tr>
 </table>
+-->
 
 # Terminology
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
@@ -338,38 +365,53 @@
 <th align="center">
 <a href="https://opensource.fb.com/"><img src="docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
 <a href="https://pytorch.org/"><img src="docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="docs/img/logo_udacity.png" /></a>
+<a href="https://www.dpmc.govt.nz/">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_nz_dark.png">
+  <img src="docs/img/logo_nz_light.png" />
+</picture>
+</a>
+</th>
+<th align="center">
+<a href="https://twitter.com/"><img src="docs/img/logo_twitter.png" /></a>
+</th>
+<th align="center">
+<a href="https://google.com/"><img src="docs/img/logo_google.png" /></a>
+</th>
+<th align="center">
+<a href="https://microsoft.com/"><img src="docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://summerofcode.withgoogle.com/"><img src="docs/img/logo_gsoc.png" /></a>
+<a href="https://omidyar.com/"><img src="docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://developers.google.com/season-of-docs"><img src="docs/img/logo_gsod.png" /></a>
+<a href="https://www.udacity.com/"><img src="docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
+<a href="https://www.centerfordigitalhealthinnovation.org/">
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
-  <img src="docs/img/logo_arkhn_light.png" />
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cdhi_dark.png">
+  <img src="docs/img/logo_cdhi_light.png" />
 </picture>
 
+</a>
 </th>
 <th align="center">
+<a href="https://arkhn.org/">
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cape.png">
-  <img src="docs/img/logo_cape_light.png" />
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
+  <img src="docs/img/logo_arkhn_light.png" />
 </picture>
-</th>
-<th align="center">
-<a href="https://begin.ai/"><img src="docs/img/logo_begin.png" /></a>
+</a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
```

#### html2text {}

```diff
@@ -1,54 +1,58 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b9 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b1 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
-Provides-Extra: oblv License-File: LICENSE
+charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
+Provides-Extra: test_plugins Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
-  [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
-else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
-Install syft on Python 3.9 - 3.11 ```bash $ pip install -U syft -f https://
-whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
-Domain ```python # from Jupyter / Python import syft as sy sy.requires
-(">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
-dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
---name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
-8080 ``` ## Connect with our Python Client ```python import syft as sy
-sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
-email="info@openmined.org", password="changethis") ``` ## Deploy to a Container
-Engine or Cloud 1. Install our handy ðµ cli tool which makes deploying a
-Domain or Gateway server a one-liner: `pip install -U hagrid` 2. Then run our
+  [Syft Logo]  Perform data science on `data` that remains in `someone else's`
+server # Quickstart â `Linux` â `macOS` â `Windows`\* â `Docker` â
+`Kubernetes` ## Install Client ```bash $ pip install -U syft -f https://
+whls.blob.core.windows.net/unstable/index.html ``` ## Launch Server ```python #
+from Jupyter / Python import syft as sy sy.requires(">=0.8.1,<0.8.2") node =
+sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True) ```
+```bash # or from the command line $ syft launch --name=my-domain --port=8080 -
+-reset=True Starting syft-node server on 0.0.0.0:8080 ``` ## Launch Client
+```python import syft as sy sy.requires(">=0.8.1,<0.8.2") domain_client =
+sy.login(port=8080, email="info@openmined.org", password="changethis") ``` ##
+PySyft in 10 minutes ð API_Example_Notebooks - 00-load-data.ipynb - 01-
+submit-code.ipynb - 02-review-code-and-approve.ipynb - 03-data-scientist-
+download-result.ipynb - 04-jax-example.ipynb - 05-custom-policy.ipynb - 06-
+multiple-code-requests.ipynb - 07-domain-register-control-flow.ipynb ## Deploy
+Kubernetes Helm Chart ``` $ kubectl create namespace syft $ helm install my-
+domain syft --namespace syft --version 0.8.1 --repo https://
+openmined.github.io/PySyft/helm ``` ### Azure or GCP Ingress ``` $ helm install
+... --set ingress.ingressClass="azure/application-gateway" $ helm install ... -
+-set ingress.ingressClass="gce" ``` ## Deploy to a Container Engine or Cloud 1.
+Install our handy ðµ cli tool which makes deploying a Domain or Gateway
+server to Docker or VM a one-liner: `pip install -U hagrid` 2. Then run our
 interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart`
 3. In the tutorial you will learn how to install and deploy: `PySyft` = our
 `numpy`-like ð Python library for computing on `private data` in someone
 else's `Domain` `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway`
-Servers where `private data` lives 4. During quickstart we will deploy `PyGrid`
-to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
-a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
-`ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
-`#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
-`git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
-WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
-not support `ansible`, preventing some remote deployment targets - PySyft 0.8
-Requires: ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`macOS` Apple
-Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
+Servers where `private data` lives ## Docs and Support - ð Docs - `#support`
+on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run:
+`pip install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA
+Requires ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires:
+ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`Windows` users must
 run this first: `pip install jaxlib==0.4.10 -f https://
 whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
-`docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
-(Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
-- Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
+`docker`, â¸ï¸ `kubernetes` or ð§ `ubuntu` VM - Run: `hagrid launch ...` #
+Versions `0.9.0` - Coming soon... `0.8.2` (Beta) - `dev` branch ðð½ API -
+Coming soon... `0.8.1` (Stable) - API Deprecated: - `0.8.0` - API - `0.7.0` -
+Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
 context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
 ... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
 `hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
 version of `hagrid` is usually the best. # What is Syft?   [Syft]  `Syft` is
 OpenMined's `open source` stack that provides `secure` and `private` Data
@@ -66,27 +70,16 @@
 Data Science`. It means in a wide variety of `domains` across society, the
 current `risks` of sharing information (`copying` data) with someone such as,
 privacy invasion, IP theft and blackmail will no longer prevent the vast
 `benefits` such as innovation, insights and scientific discovery which secure
 access will provide. No more cold calls to get `access` to a dataset. No more
 weeks of `wait times` to get a `result` on your `query`. It also means `1000x
 more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Tutorials
- _____________________________________________________________________________
-|             [Image]     |            [Image]      |            [Image]      |
-|___________Data_Owner____|________Data_Scientist___|_________Data_Engineer___|
-|- Deploy_a_Domain_Server |- Install Syft           |- Setup Dev Mode         |
-|- Upload_Private_Data -  | - Connect to a Domain   | - Deploy to Azure -     |
-|Create_Accounts - Manage | - Search for Datasets   |Deploy to GCP - Deploy to|
-|Privacy Budget           | - Train Models -        |Kubernetes - Customize   |
-| - Join_a_Network - Learn|Retrieve Secure Results -|Networking - Modify      |
-|how PETs streamline Data |Learn Differential       |PyGrid UI                |
-|Policies_________________|Privacy__________________|_________________________|
-# Terminology
+Scientist `workflow`, all with the individual's `privacy` at its heart.  #
+Terminology
  _________________________________________________________________________________________
 |                 [Image]                  |                   [Image]                    |
 |_______ð¨ð»âð¼_Data|_______ð©ð½âð¬_Data_Sci|ntists
 | Provide `datasets` which they would like | Are end `users` who desire to perform        |
 |to make available for `study` by an       |`computations` or `answer` a specific         |
 |`outside party` they may or may not `fully|`question` using one or more data owners'     |
 |trust`_has_good_intentions._______________|`datasets`.___________________________________|
@@ -116,16 +109,16 @@
 # Courses
  _______________________
 |[Image]|[Image]|[Image]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
   [Contributors]  # Supporters
-  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/         [docs/img/            [docs/img/       [docs/img/
-logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] logo_arkhn_light.png] logo_cape_light.png] logo_begin.png]
+  [docs/img/      [docs/img/     [docs/img/       __[docs/img/       [docs/img/        [docs/img/        [docs/img/       [docs/img/     [docs/img/         __[docs/img/         __[docs/img/
+logo_sloan.png] logo_meta.png] logo_torch.png] logo_nz_light.png] logo_twitter.png] logo_google.png] logo_microsoft.png] logo_on.png] logo_udacity.png] logo_cdhi_light.png] logo_arkhn_light.png]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on Open_Collective.
 
   [Contributors]  # Disclaimer Syft is under active development and is not yet
 ready for pilots on private data without our assistance. As early access
 participants, please contact us via [Slack](https://slack.openmined.org/) or
 email if you would like to ask a question or have a use case that you would
```

### Comparing `syft-0.8.1b9/README.md` & `syft-0.8.2b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,88 +2,112 @@
 <br /><br /></div>
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
-Perform `numpy`-like analysis on `data` that remains in `someone else's` server
+Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
+✅ `Linux` ✅ `macOS` ✅ `Windows`\* ✅ `Docker` ✅ `Kubernetes`
 
-## Install syft on Python 3.9 - 3.11
+## Install Client
 
 ```bash
 $ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
-## Launch a python dev Domain
+## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8,<0.8.1")
+sy.requires(">=0.8.1,<0.8.2")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
-## Connect with our Python Client
+## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8,<0.8.1")
+sy.requires(">=0.8.1,<0.8.2")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
+## PySyft in 10 minutes
+
+📝 <a href="/notebooks/api">API Example Notebooks</a>
+
+- <a href="/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+
+## Deploy Kubernetes Helm Chart
+
+```
+$ kubectl create namespace syft
+$ helm install my-domain syft --namespace syft --version 0.8.1 --repo https://openmined.github.io/PySyft/helm
+```
+
+### Azure or GCP Ingress
+
+```
+$ helm install ... --set ingress.ingressClass="azure/application-gateway"
+$ helm install ... --set ingress.ingressClass="gce"
+```
+
 ## Deploy to a Container Engine or Cloud
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
+1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
    `pip install -U hagrid`
 
 2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
    `hagrid quickstart`
 
 3. In the tutorial you will learn how to install and deploy:  
    `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
 
    `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
-4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
-
 ## Docs and Support
 
-- 📝 <a href="/notebooks/api">API Example Notebooks</a>
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
-  †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
-  \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
-  ‡`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
-- PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
+- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
+- PySyft 0.8.1 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
+  \*`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
+- PyGrid Requires: 🐳 `docker`, ☸️ `kubernetes` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
-`0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
+`0.9.0` - Coming soon...  
+`0.8.2` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.1` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
@@ -106,14 +130,15 @@
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
 No more cold calls to get `access` to a dataset. No more weeks of `wait times` to get a `result` on your `query`. It also means `1000x more data` in every domain. PySyft opens the doors to a streamlined Data Scientist `workflow`, all with the individual's `privacy` at its heart.
 
+<!--
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
@@ -162,14 +187,15 @@
 - Deploy to GCP
 - Deploy to Kubernetes
 - Customize Networking
 - Modify PyGrid UI
 </td>
 </tr>
 </table>
+-->
 
 # Terminology
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
@@ -318,38 +344,53 @@
 <th align="center">
 <a href="https://opensource.fb.com/"><img src="docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
 <a href="https://pytorch.org/"><img src="docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="docs/img/logo_udacity.png" /></a>
+<a href="https://www.dpmc.govt.nz/">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_nz_dark.png">
+  <img src="docs/img/logo_nz_light.png" />
+</picture>
+</a>
+</th>
+<th align="center">
+<a href="https://twitter.com/"><img src="docs/img/logo_twitter.png" /></a>
+</th>
+<th align="center">
+<a href="https://google.com/"><img src="docs/img/logo_google.png" /></a>
+</th>
+<th align="center">
+<a href="https://microsoft.com/"><img src="docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://summerofcode.withgoogle.com/"><img src="docs/img/logo_gsoc.png" /></a>
+<a href="https://omidyar.com/"><img src="docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://developers.google.com/season-of-docs"><img src="docs/img/logo_gsod.png" /></a>
+<a href="https://www.udacity.com/"><img src="docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
+<a href="https://www.centerfordigitalhealthinnovation.org/">
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
-  <img src="docs/img/logo_arkhn_light.png" />
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cdhi_dark.png">
+  <img src="docs/img/logo_cdhi_light.png" />
 </picture>
 
+</a>
 </th>
 <th align="center">
+<a href="https://arkhn.org/">
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cape.png">
-  <img src="docs/img/logo_cape_light.png" />
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
+  <img src="docs/img/logo_arkhn_light.png" />
 </picture>
-</th>
-<th align="center">
-<a href="https://begin.ai/"><img src="docs/img/logo_begin.png" /></a>
+</a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
```

#### html2text {}

```diff
@@ -1,45 +1,49 @@
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
-  [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
-else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
-Install syft on Python 3.9 - 3.11 ```bash $ pip install -U syft -f https://
-whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
-Domain ```python # from Jupyter / Python import syft as sy sy.requires
-(">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
-dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
---name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
-8080 ``` ## Connect with our Python Client ```python import syft as sy
-sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
-email="info@openmined.org", password="changethis") ``` ## Deploy to a Container
-Engine or Cloud 1. Install our handy ðµ cli tool which makes deploying a
-Domain or Gateway server a one-liner: `pip install -U hagrid` 2. Then run our
+  [Syft Logo]  Perform data science on `data` that remains in `someone else's`
+server # Quickstart â `Linux` â `macOS` â `Windows`\* â `Docker` â
+`Kubernetes` ## Install Client ```bash $ pip install -U syft -f https://
+whls.blob.core.windows.net/unstable/index.html ``` ## Launch Server ```python #
+from Jupyter / Python import syft as sy sy.requires(">=0.8.1,<0.8.2") node =
+sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True) ```
+```bash # or from the command line $ syft launch --name=my-domain --port=8080 -
+-reset=True Starting syft-node server on 0.0.0.0:8080 ``` ## Launch Client
+```python import syft as sy sy.requires(">=0.8.1,<0.8.2") domain_client =
+sy.login(port=8080, email="info@openmined.org", password="changethis") ``` ##
+PySyft in 10 minutes ð API_Example_Notebooks - 00-load-data.ipynb - 01-
+submit-code.ipynb - 02-review-code-and-approve.ipynb - 03-data-scientist-
+download-result.ipynb - 04-jax-example.ipynb - 05-custom-policy.ipynb - 06-
+multiple-code-requests.ipynb - 07-domain-register-control-flow.ipynb ## Deploy
+Kubernetes Helm Chart ``` $ kubectl create namespace syft $ helm install my-
+domain syft --namespace syft --version 0.8.1 --repo https://
+openmined.github.io/PySyft/helm ``` ### Azure or GCP Ingress ``` $ helm install
+... --set ingress.ingressClass="azure/application-gateway" $ helm install ... -
+-set ingress.ingressClass="gce" ``` ## Deploy to a Container Engine or Cloud 1.
+Install our handy ðµ cli tool which makes deploying a Domain or Gateway
+server to Docker or VM a one-liner: `pip install -U hagrid` 2. Then run our
 interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart`
 3. In the tutorial you will learn how to install and deploy: `PySyft` = our
 `numpy`-like ð Python library for computing on `private data` in someone
 else's `Domain` `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway`
-Servers where `private data` lives 4. During quickstart we will deploy `PyGrid`
-to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
-a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
-`ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
-`#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
-`git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
-WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
-not support `ansible`, preventing some remote deployment targets - PySyft 0.8
-Requires: ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`macOS` Apple
-Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
+Servers where `private data` lives ## Docs and Support - ð Docs - `#support`
+on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run:
+`pip install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA
+Requires ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires:
+ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`Windows` users must
 run this first: `pip install jaxlib==0.4.10 -f https://
 whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
-`docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
-(Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
-- Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
+`docker`, â¸ï¸ `kubernetes` or ð§ `ubuntu` VM - Run: `hagrid launch ...` #
+Versions `0.9.0` - Coming soon... `0.8.2` (Beta) - `dev` branch ðð½ API -
+Coming soon... `0.8.1` (Stable) - API Deprecated: - `0.8.0` - API - `0.7.0` -
+Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
 context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
 ... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
 `hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
 version of `hagrid` is usually the best. # What is Syft?   [Syft]  `Syft` is
 OpenMined's `open source` stack that provides `secure` and `private` Data
@@ -57,27 +61,16 @@
 Data Science`. It means in a wide variety of `domains` across society, the
 current `risks` of sharing information (`copying` data) with someone such as,
 privacy invasion, IP theft and blackmail will no longer prevent the vast
 `benefits` such as innovation, insights and scientific discovery which secure
 access will provide. No more cold calls to get `access` to a dataset. No more
 weeks of `wait times` to get a `result` on your `query`. It also means `1000x
 more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Tutorials
- _____________________________________________________________________________
-|             [Image]     |            [Image]      |            [Image]      |
-|___________Data_Owner____|________Data_Scientist___|_________Data_Engineer___|
-|- Deploy_a_Domain_Server |- Install Syft           |- Setup Dev Mode         |
-|- Upload_Private_Data -  | - Connect to a Domain   | - Deploy to Azure -     |
-|Create_Accounts - Manage | - Search for Datasets   |Deploy to GCP - Deploy to|
-|Privacy Budget           | - Train Models -        |Kubernetes - Customize   |
-| - Join_a_Network - Learn|Retrieve Secure Results -|Networking - Modify      |
-|how PETs streamline Data |Learn Differential       |PyGrid UI                |
-|Policies_________________|Privacy__________________|_________________________|
-# Terminology
+Scientist `workflow`, all with the individual's `privacy` at its heart.  #
+Terminology
  _________________________________________________________________________________________
 |                 [Image]                  |                   [Image]                    |
 |_______ð¨ð»âð¼_Data|_______ð©ð½âð¬_Data_Sci|ntists
 | Provide `datasets` which they would like | Are end `users` who desire to perform        |
 |to make available for `study` by an       |`computations` or `answer` a specific         |
 |`outside party` they may or may not `fully|`question` using one or more data owners'     |
 |trust`_has_good_intentions._______________|`datasets`.___________________________________|
@@ -107,16 +100,16 @@
 # Courses
  _______________________
 |[Image]|[Image]|[Image]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
   [Contributors]  # Supporters
-  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/         [docs/img/            [docs/img/       [docs/img/
-logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] logo_arkhn_light.png] logo_cape_light.png] logo_begin.png]
+  [docs/img/      [docs/img/     [docs/img/       __[docs/img/       [docs/img/        [docs/img/        [docs/img/       [docs/img/     [docs/img/         __[docs/img/         __[docs/img/
+logo_sloan.png] logo_meta.png] logo_torch.png] logo_nz_light.png] logo_twitter.png] logo_google.png] logo_microsoft.png] logo_on.png] logo_udacity.png] logo_cdhi_light.png] logo_arkhn_light.png]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on Open_Collective.
 
   [Contributors]  # Disclaimer Syft is under active development and is not yet
 ready for pilots on private data without our assistance. As early access
 participants, please contact us via [Slack](https://slack.openmined.org/) or
 email if you would like to ask a question or have a use case that you would
```

### Comparing `syft-0.8.1b9/setup.cfg` & `syft-0.8.2b1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.9"
+version = attr: "0.8.2-beta.1"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -19,73 +19,75 @@
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 syft = 
-	astunparse==1.6.3
 	bcrypt==4.0.1
 	forbiddenfruit==0.1.4
 	gevent==22.10.2
 	gipc==1.5.0
 	jax==0.4.10
 	jaxlib==0.4.10
 	loguru==0.7.0
 	networkx==2.8
-	numpy==1.24.3
-	opendp==0.6.2
+	numpy>=1.22.4,<=1.24.3
+	opendp==0.7.0
 	packaging>=21.0
 	pandas==1.5.3
 	pyarrow==11.0.0
 	pycapnp==1.3.0
 	pydantic[email]==1.10.7
 	pymongo==4.3.3
 	pynacl==1.5.0
-	pyzmq==23.2.1
-	redis==4.5.4
-	requests==2.29.0
+	pyzmq>=23.2.1,<=25.1.0
+	redis==4.5.5
+	requests==2.31.0
 	RestrictedPython==6.0
-	result==0.9.0
+	result==0.10.0
 	tqdm==4.65.0
 	typeguard==2.13.3
-	typing_extensions==4.5.0
+	typing_extensions==4.6.3
 	sherlock[redis,filelock]==0.4.1
-	uvicorn[standard]==0.21.1
-	fastapi==0.95.1
+	uvicorn[standard]==0.22.0
+	fastapi==0.97.0
 	hagrid>=0.3
 	matplotlib==3.7.1
 	dm-haiku==0.0.9
-	itables==1.5.2
-telemetry = 
-	opentelemetry-api==1.14.0
-	opentelemetry-sdk==1.14.0
-	opentelemetry-exporter-jaeger==1.14.0
-	opentelemetry-instrumentation==0.35b0
-	opentelemetry-instrumentation-requests==0.35b0
+	itables==1.5.3
+	transformers==4.30.2
+	evaluate==0.4.0
+	torch==2.0.1
 install_requires = 
 	%(syft)s
-	%(telemetry)s
 python_requires = >=3.9
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 dev = 
 	%(test_plugins)s
+	%(telemetry)s
 	bandit==1.7.5
 	ruff==0.0.254
 	importlib-metadata==6.0.0
 	isort==5.12.0
 	mypy==1.1.1
 	pre-commit==3.1.1
 	safety==2.3.5
+telemetry = 
+	opentelemetry-api==1.14.0
+	opentelemetry-sdk==1.14.0
+	opentelemetry-exporter-jaeger==1.14.0
+	opentelemetry-instrumentation==0.35b0
+	opentelemetry-instrumentation-requests==0.35b0
 test_plugins = 
 	pytest
 	pytest-cov
 	pytest-xdist[psutil]
 	pytest-parallel
 	pytest-asyncio
 	pytest-randomly
```

### Comparing `syft-0.8.1b9/src/syft/VERSION` & `syft-0.8.2b1/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.9"
+__version__ = "0.8.2-beta.1"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b9/src/syft/__init__.py` & `syft-0.8.2b1/src/syft/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-__version__ = "0.8.1-beta.9"
+__version__ = "0.8.2-beta.1"
 
 # stdlib
+import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
 # relative
 from . import gevent_patch  # noqa: F401
 from .client.client import connect  # noqa: F401
 from .client.client import login  # noqa: F401
+from .client.client import register  # noqa: F401
 from .client.deploy import Orchestra  # noqa: F401
 from .client.registry import DomainRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
 from .client.search import Search  # noqa: F401
 from .client.search import SearchResults  # noqa: F401
 from .client.user_settings import UserSettings  # noqa: F401
 from .client.user_settings import settings  # noqa: F401
@@ -29,16 +31,17 @@
 from .serde.deserialize import _deserialize as deserialize  # noqa: F401
 from .serde.serializable import serializable  # noqa: F401
 from .serde.serialize import _serialize as serialize  # noqa: F401
 from .service.action.action_data_empty import ActionDataEmpty  # noqa: F401
 from .service.action.action_object import ActionObject  # noqa: F401
 from .service.action.plan import Plan  # noqa: F401
 from .service.action.plan import planify  # noqa: F401
-from .service.code.user_code import UserCodeStatus  # noqa: F401
-from .service.code.user_code import syft_function  # noqa: F401
+from .service.code.user_code import UserCodeStatus  # noqa: F401; noqa: F401
+from .service.code.user_code import syft_function  # noqa: F401; noqa: F401
+from .service.code.user_code import syft_function_single_use  # noqa: F401; noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .service.dataset.dataset import Contributor  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
 from .service.dataset.dataset import CreateDataset as Dataset  # noqa: F401
 from .service.message.messages import MessageStatus  # noqa: F401
 from .service.policy.policy import CustomInputPolicy  # noqa: F401
 from .service.policy.policy import CustomOutputPolicy  # noqa: F401
@@ -54,28 +57,45 @@
 from .service.user.roles import Roles as roles  # noqa: F401
 from .service.user.user_service import UserService  # noqa: F401
 from .types.twin_object import TwinObject  # noqa: F401
 from .types.uid import UID  # noqa: F401
 from .util import filterwarnings  # noqa: F401
 from .util import jax_settings  # noqa: F401
 from .util import logger  # noqa: F401
+from .util import options  # noqa: F401
 from .util.autoreload import disable_autoreload  # noqa: F401
 from .util.autoreload import enable_autoreload  # noqa: F401
 from .util.telemetry import instrument  # noqa: F401
 from .util.util import autocache  # noqa: F401
 from .util.util import get_root_data_path  # noqa: F401
 from .util.version_compare import make_requires
 
-LATEST_STABLE_SYFT = "0.8"
+LATEST_STABLE_SYFT = "0.8.1"
 requires = make_requires(LATEST_STABLE_SYFT, __version__)
 
+
+# SYFT_PATH = path = os.path.abspath(a_module.__file__)
+SYFT_PATH = pathlib.Path(__file__).parent.resolve()
+
 sys.path.append(str(Path(__file__)))
 
 logger.start()
 
+try:
+    get_ipython()  # noqa: F821
+    # TODO: add back later or auto detect
+    # display(
+    #     Markdown(
+    #         "\nWarning: syft is imported in light mode by default. \
+    #     \nTo switch to dark mode, please run `sy.options.color_theme = 'dark'`"
+    #     )
+    # )
+except:  # noqa: E722
+    pass  # nosec
+
 # For server-side, to enable by environment variable
 if OBLV:
     enable_external_lib("oblv")
 
 
 def module_property(func: Any) -> Callable:
     """Decorator to turn module functions into properties.
```

### Comparing `syft-0.8.1b9/src/syft/abstract_node.py` & `syft-0.8.2b1/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/client/api.py` & `syft-0.8.2b1/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/client/client.py` & `syft-0.8.2b1/src/syft/client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,34 +22,38 @@
 from requests.packages.urllib3.util.retry import Retry
 from tqdm import tqdm
 from typing_extensions import Self
 
 # relative
 from .. import __version__
 from ..abstract_node import AbstractNode
+from ..img.base64 import base64read
 from ..node.credentials import SyftSigningKey
 from ..node.credentials import SyftVerifyKey
 from ..node.credentials import UserLoginCredentials
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..service.context import NodeServiceContext
 from ..service.dataset.dataset import CreateDataset
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
+from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..types.grid_url import GridURL
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.uid import UID
+from ..util.fonts import fonts_css
 from ..util.logger import debug
 from ..util.telemetry import instrument
+from ..util.util import get_mb_size
 from ..util.util import thread_ident
 from ..util.util import verify_tls
 from .api import APIModule
 from .api import APIRegistry
 from .api import SignedSyftAPICall
 from .api import SyftAPI
 from .api import SyftAPICall
@@ -189,15 +193,15 @@
         return cast(SyftAPI, obj)
 
     def login(self, email: str, password: str) -> Optional[SyftSigningKey]:
         credentials = {"email": email, "password": password}
         response = self._make_post(self.routes.ROUTE_LOGIN.value, credentials)
         obj = _deserialize(response, from_bytes=True)
         if isinstance(obj, UserPrivateKey):
-            return obj.signing_key
+            return obj
         return None
 
     def register(self, new_user: UserCreate) -> SyftSigningKey:
         data = _serialize(new_user, to_bytes=True)
         response = self._make_post(self.routes.ROUTE_REGISTER.value, data=data)
         response = _deserialize(response, from_bytes=True)
         return response
@@ -278,15 +282,15 @@
         )
         result = method()
         return result
 
     def login(self, email: str, password: str) -> Optional[SyftSigningKey]:
         obj = self.exchange_credentials(email=email, password=password)
         if isinstance(obj, UserPrivateKey):
-            return obj.signing_key
+            return obj
         return None
 
     def register(self, new_user: UserCreate) -> Optional[SyftSigningKey]:
         service_context = NodeServiceContext(node=self.node)
         method = self.node.get_service_method(UserService.register)
         response = method(context=service_context, new_user=new_user)
         return response
@@ -304,14 +308,15 @@
 @instrument
 @serializable()
 class SyftClient:
     connection: NodeConnection
     metadata: Optional[NodeMetadataJSON]
     credentials: Optional[SyftSigningKey]
     __logged_in_user: str = ""
+    __user_role: ServiceRole = ServiceRole.NONE
 
     def __init__(
         self,
         connection: NodeConnection,
         metadata: Optional[NodeMetadataJSON] = None,
         credentials: Optional[SyftSigningKey] = None,
         api: Optional[SyftAPI] = None,
@@ -332,14 +337,18 @@
         return bool(self.credentials)
 
     @property
     def logged_in_user(self) -> Optional[str]:
         return self.__logged_in_user
 
     @property
+    def user_role(self) -> ServiceRole:
+        return self.__user_role
+
+    @property
     def verify_key(self) -> SyftVerifyKey:
         if self.credentials is None:
             raise ValueError("SigningKey not set on client")
         return self.credentials.verify_key
 
     @staticmethod
     def from_url(url: Union[str, GridURL]) -> Self:
@@ -366,36 +375,41 @@
         # invalidate API
         if self._api is None or (self._api.signing_key != self.credentials):
             self._fetch_api(self.credentials)
 
         return self._api
 
     def guest(self) -> Self:
-        self.credentials = SyftSigningKey.generate()
-        self.__logged_in_user = ""
-        return self
+        return SyftClient(
+            connection=self.connection,
+            credentials=SyftSigningKey.generate(),
+            metadata=self.metadata,
+        )
 
     def upload_dataset(self, dataset: CreateDataset) -> Union[SyftSuccess, SyftError]:
         # relative
         from ..types.twin_object import TwinObject
 
         dataset._check_asset_must_contain_mock()
+        dataset_size = 0
 
         for asset in tqdm(dataset.asset_list):
             print(f"Uploading: {asset.name}")
             try:
                 twin = TwinObject(private_obj=asset.data, mock_obj=asset.mock)
             except Exception as e:
                 return SyftError(message=f"Failed to create twin. {e}")
             response = self.api.services.action.set(twin)
             if isinstance(response, SyftError):
                 print(f"Failed to upload asset\n: {asset}")
                 return response
             asset.action_id = twin.id
             asset.node_uid = self.id
+            dataset_size += get_mb_size(asset.data)
+        dataset.mb_size = dataset_size
         valid = dataset.check()
         if valid.ok():
             return self.api.services.dataset.add(dataset=dataset)
         else:
             if len(valid.err()) > 0:
                 return tuple(valid.err())
             return valid.err()
@@ -427,14 +441,20 @@
     @property
     def users(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("user"):
             return self.api.services.user
         return None
 
     @property
+    def settings(self) -> Optional[APIModule]:
+        if self.api is not None and self.api.has_service("user"):
+            return self.api.services.settings
+        return None
+
+    @property
     def code(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("code"):
             return self.api.services.code
 
     @property
     def requests(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("request"):
@@ -445,14 +465,18 @@
     def datasets(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("dataset"):
             return self.api.services.dataset
         return None
 
     @property
     def notifications(self) -> Optional[APIModule]:
+        print(
+            "WARNING: Notifications is currently is in a beta state, so use carefully!"
+        )
+        print("If possible try using client.requests/client.projects")
         if self.api is not None and self.api.has_service("messages"):
             return self.api.services.messages
         return None
 
     @property
     def domains(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("network"):
@@ -480,19 +504,26 @@
 
         elif uid:
             return self.api.services.project.get_by_uid(uid)
 
         return self.api.services.project.get_all()
 
     def login(self, email: str, password: str, cache: bool = True) -> Self:
-        signing_key = self.connection.login(email=email, password=password)
+        user_private_key = self.connection.login(email=email, password=password)
+        signing_key = None
+        if user_private_key is not None:
+            signing_key = user_private_key.signing_key
+            self.__user_role = user_private_key.role
         if signing_key is not None:
             self.credentials = signing_key
             self.__logged_in_user = email
+            # TODO: How to get the role of the user?
+            # self.__user_role =
             self._fetch_api(self.credentials)
+            print(f"Logged into {self.name} as <{email}>")
             if cache:
                 SyftClientSessionCache.add_client(
                     email=email,
                     password=password,
                     connection=self.connection,
                     syft_client=self,
                 )
@@ -535,14 +566,15 @@
             new_user = UserCreate(
                 name=name,
                 email=email,
                 password=password,
                 password_verify=password,
                 institution=institution,
                 website=website,
+                created_by=self.credentials,
             )
         except Exception as e:
             return SyftError(message=str(e))
         response = self.connection.register(new_user=new_user)
         if isinstance(response, tuple):
             response = response[0]
         return response
@@ -598,14 +630,108 @@
         uid = self.id
         if proxy_target_uid:
             client_type = "ProxyClient"
             uid = proxy_target_uid
             return f"<{client_type} - <{uid}>: via {self.id} {self.connection}>"
         return f"<{client_type} - {self.name} <{uid}>: {self.connection}>"
 
+    def _repr_html_(self) -> str:
+        guest_commands = """
+        <li><span class='syft-code-block'>&lt;your_client&gt;.datasets</span> - list datasets</li>
+        <li><span class='syft-code-block'>&lt;your_client&gt;.code</span> - list code</li>
+        <li><span class='syft-code-block'>&lt;your_client&gt;.login</span> - list projects</li>
+        <li>
+            <span class='syft-code-block'>&lt;your_client&gt;.code.submit?</span> - display function signature
+        </li>"""
+        ds_commands = """
+        <li><span class='syft-code-block'>&lt;your_client&gt;.datasets</span> - list datasets</li>
+        <li><span class='syft-code-block'>&lt;your_client&gt;.code</span> - list code</li>
+        <li><span class='syft-code-block'>&lt;your_client&gt;.projects</span> - list projects</li>
+        <li>
+            <span class='syft-code-block'>&lt;your_client&gt;.code.submit?</span> - display function signature
+        </li>"""
+
+        do_commands = """
+        <li><span class='syft-code-block'>&lt;your_client&gt;.projects</span> - list projects</li>
+        <li><span class='syft-code-block'>&lt;your_client&gt;.requests</span> - list requests</li>
+        <li><span class='syft-code-block'>&lt;your_client&gt;.users</span> - list users</li>
+        <li>
+            <span class='syft-code-block'>&lt;your_client&gt;.requests.submit?</span> - display function signature
+        </li>"""
+
+        # TODO: how to select ds/do commands based on self.__user_role
+
+        if (
+            self.user_role.value == ServiceRole.NONE.value
+            or self.user_role.value == ServiceRole.GUEST.value
+        ):
+            commands = guest_commands
+        elif (
+            self.user_role is not None
+            and self.user_role.value == ServiceRole.DATA_SCIENTIST.value
+        ):
+            commands = ds_commands
+        elif (
+            self.user_role is not None
+            and self.user_role.value >= ServiceRole.DATA_OWNER.value
+        ):
+            commands = do_commands
+
+        command_list = f"""
+        <ul style='padding-left: 1em;'>
+            {commands}
+        </ul>
+        """
+
+        small_grid_symbol_logo = base64read("small-grid-symbol-logo.png")
+
+        return f"""
+        <style>
+            {fonts_css}
+
+            .syft-container {{
+                padding: 5px;
+                font-family: 'Open Sans';
+            }}
+            .syft-alert-info {{
+                color: #1F567A;
+                background-color: #C2DEF0;
+                border-radius: 4px;
+                padding: 5px;
+                padding: 13px 10px
+            }}
+            .syft-code-block {{
+                background-color: #f7f7f7;
+                border: 1px solid #cfcfcf;
+                padding: 0px 2px;
+            }}
+            .syft-space {{
+                margin-top: 1em;
+            }}
+        </style>
+        <div class="syft-client syft-container">
+            <img src="{small_grid_symbol_logo}" alt="Logo"
+            style="width:48px;height:48px;padding:3px;">
+            <h2>Welcome to {self.name}</h2>
+            <div class="syft-space">
+                <!-- <strong>Institution:</strong> TODO<br /> -->
+                <!-- <strong>Owner:</strong> TODO<br /> -->
+                <strong>URL:</strong> {getattr(self.connection, 'url', '')}<br />
+                <!-- <strong>PyGrid Admin:</strong> TODO<br /> -->
+            </div>
+            <div class='syft-alert-info syft-space'>
+                &#9432;&nbsp;
+                This domain is run by the library PySyft to learn more about how it works visit
+                <a href="https://github.com/OpenMined/PySyft">github.com/OpenMined/PySyft</a>.
+            </div>
+            <h4>Commands to Get Started</h4>
+            {command_list}
+        </div><br />
+        """
+
     def _fetch_node_metadata(self, credentials: SyftSigningKey) -> None:
         metadata = self.connection.get_node_metadata(credentials=credentials)
         if isinstance(metadata, NodeMetadataJSON):
             metadata.check_version(__version__)
             self.metadata = metadata
 
     def _fetch_api(self, credentials: SyftSigningKey):
@@ -637,29 +763,55 @@
             url.set_port(int(port))
         connection = HTTPConnection(url=url)
     _client = SyftClient(connection=connection)
     return _client
 
 
 @instrument
+def register(
+    url: Union[str, GridURL],
+    port: int,
+    name: str,
+    email: str,
+    password: str,
+    institution: Optional[str] = None,
+    website: Optional[str] = None,
+):
+    guest_client = connect(url=url, port=port)
+    return guest_client.register(
+        name=name,
+        email=email,
+        password=password,
+        institution=institution,
+        website=website,
+    )
+
+
+@instrument
 def login(
     url: Union[str, GridURL] = DEFAULT_PYGRID_ADDRESS,
     node: Optional[AbstractNode] = None,
     port: Optional[int] = None,
     email: Optional[str] = None,
     password: Optional[str] = None,
     cache: bool = True,
+    verbose: bool = True,
 ) -> SyftClient:
     _client = connect(url=url, node=node, port=port)
     connection = _client.connection
 
     login_credentials = None
     if email and password:
         login_credentials = UserLoginCredentials(email=email, password=password)
 
+    if login_credentials is None:
+        if verbose:
+            print(f"Logged into {_client.name} as GUEST")
+        return _client.guest()
+
     if cache and login_credentials:
         _client_cache = SyftClientSessionCache.get_client(
             login_credentials.email,
             login_credentials.password,
             connection=connection,
         )
         if _client_cache:
@@ -670,17 +822,15 @@
 
     if not _client.authed and login_credentials:
         _client.login(
             email=login_credentials.email,
             password=login_credentials.password,
             cache=cache,
         )
-        if _client.authed:
-            print(f"Logged into {_client.name} as <{login_credentials.email}>")
-        else:
+        if not _client.authed:
             return SyftError(message=f"Failed to login as {login_credentials.email}")
 
     return _client
 
 
 class SyftClientSessionCache:
     __credentials_store__: Dict = {}
```

### Comparing `syft-0.8.1b9/src/syft/client/connection.py` & `syft-0.8.2b1/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/client/deploy.py` & `syft-0.8.2b1/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/client/registry.py` & `syft-0.8.2b1/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/client/search.py` & `syft-0.8.2b1/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/client/user_settings.py` & `syft-0.8.2b1/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/__init__.py` & `syft-0.8.2b1/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/__init__.py` & `syft-0.8.2b1/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/deployment.py` & `syft-0.8.2b1/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b1/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b1/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b1/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b1/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b1/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/gevent_patch.py` & `syft-0.8.2b1/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/node/credentials.py` & `syft-0.8.2b1/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/node/gateway.py` & `syft-0.8.2b1/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/node/node.py` & `syft-0.8.2b1/src/syft/node/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,18 @@
 from ..store.document_store import StoreConfig
 from ..store.sqlite_document_store import SQLiteStoreClientConfig
 from ..store.sqlite_document_store import SQLiteStoreConfig
 from ..types.syft_object import HIGHEST_SYFT_OBJECT_VERSION
 from ..types.syft_object import LOWEST_SYFT_OBJECT_VERSION
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
+from ..util.experimental_flags import flags
 from ..util.telemetry import instrument
 from ..util.util import random_name
+from ..util.util import str_to_bool
 from ..util.util import thread_ident
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
 from .worker_settings import WorkerSettings
 
 # if user code needs to be serded and its not available we can call this to refresh
 # the code for a specific node UID and thread
@@ -130,14 +132,20 @@
     return get_env(DEFAULT_ROOT_EMAIL, "info@openmined.org")
 
 
 def get_default_root_password() -> Optional[str]:
     return get_env(DEFAULT_ROOT_PASSWORD, "changethis")  # nosec
 
 
+def get_dev_mode() -> bool:
+    return str_to_bool(get_env("DEV_MODE", "False"))
+
+
+dev_mode = get_dev_mode()
+
 signing_key_env = get_private_key_env()
 node_uid_env = get_node_uid_env()
 
 default_root_email = get_default_root_email()
 default_root_password = get_default_root_password()
 
 
@@ -182,17 +190,14 @@
             self.signing_key = signing_key
 
         if self.signing_key is None:
             self.signing_key = SyftSigningKey.generate()
 
         self.processes = processes
         self.is_subprocess = is_subprocess
-
-        if name is None:
-            name = random_name()
         self.name = name
         services = (
             [
                 UserService,
                 SettingsService,
                 ActionService,
                 DatasetService,
@@ -319,19 +324,24 @@
         from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=self.signing_key)
 
     @property
     def guest_client(self):
+        return self.get_guest_client()
+
+    def get_guest_client(self, verbose: bool = True):
         # relative
         from ..client.client import PythonConnection
         from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
+        if verbose:
+            print(f"Logged into {self.name} as GUEST")
         return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
 
     def __repr__(self) -> str:
         service_string = ""
         if not self.is_subprocess:
             services = []
             for service in self.services:
@@ -372,17 +382,18 @@
             else:
                 document_store_config = DictStoreConfig()
         if (
             isinstance(document_store_config, SQLiteStoreConfig)
             and document_store_config.client_config.filename is None
         ):
             document_store_config.client_config.filename = f"{self.id}.sqlite"
-            print(
-                f"SQLite Store Path:\n!open file://{document_store_config.client_config.file_path}\n"
-            )
+            if dev_mode:
+                print(
+                    f"SQLite Store Path:\n!open file://{document_store_config.client_config.file_path}\n"
+                )
         document_store = document_store_config.store_type
         self.document_store_config = document_store_config
 
         self.document_store = document_store(
             root_verify_key=self.verify_key,
             store_config=document_store_config,
         )
@@ -465,27 +476,44 @@
         method_name = path_list.pop()
         service_obj = self._get_service_from_path(path=path)
 
         return getattr(service_obj, method_name)
 
     @property
     def metadata(self) -> NodeMetadata:
+        name = ""
+        deployed_on = ""
+        organization = ""
+        on_board = False
+        description = ""
+        signup_enabled = False
+
         settings_stash = SettingsStash(store=self.document_store)
-        settings = settings_stash.get_all(self.signing_key.verify_key).ok()[0]
+        settings = settings_stash.get_all(self.signing_key.verify_key)
+        if settings.is_ok() and len(settings.ok()) > 0:
+            settings_data = settings.ok()[0]
+            name = settings_data.name
+            deployed_on = settings_data.deployed_on
+            organization = settings_data.organization
+            on_board = settings_data.on_board
+            description = settings_data.description
+            signup_enabled = settings_data.signup_enabled
+
         return NodeMetadata(
-            name=settings.name,
+            name=name,
             id=self.id,
             verify_key=self.verify_key,
             highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
             lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
             syft_version=__version__,
-            deployed_on=settings.deployed_on,
-            description=settings.description,
-            organization=settings.organization,
-            on_board=settings.on_board,
+            deployed_on=deployed_on,
+            description=description,
+            organization=organization,
+            on_board=on_board,
+            signup_enabled=signup_enabled,
         )
 
     @property
     def icon(self) -> str:
         return "🦾"
 
     @property
@@ -639,23 +667,27 @@
 
     def get_unauthed_context(
         self, login_credentials: UserLoginCredentials
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
     def create_initial_settings(self) -> Optional[NodeSettings]:
+        if self.name is None:
+            self.name = random_name()
         try:
             settings_stash = SettingsStash(store=self.document_store)
             settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
             if settings_exists:
+                self.name = settings_exists[0].name
                 return None
             else:
                 new_settings = NodeSettings(
                     name=self.name,
                     deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
+                    signup_enabled=flags.CAN_REGISTER,
                 )
                 result = settings_stash.set(
                     credentials=self.signing_key.verify_key, settings=new_settings
                 )
                 if result.is_ok():
                     return result.ok()
                 return None
```

### Comparing `syft-0.8.1b9/src/syft/node/routes.py` & `syft-0.8.2b1/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/node/run.py` & `syft-0.8.2b1/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/node/server.py` & `syft-0.8.2b1/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/node/worker_settings.py` & `syft-0.8.2b1/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/array.py` & `syft-0.8.2b1/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/arrow.py` & `syft-0.8.2b1/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/deserialize.py` & `syft-0.8.2b1/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/lib_permissions.py` & `syft-0.8.2b1/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b1/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/mock.py` & `syft-0.8.2b1/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/recursive.py` & `syft-0.8.2b1/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b1/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/serializable.py` & `syft-0.8.2b1/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/signature.py` & `syft-0.8.2b1/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/serde/third_party.py` & `syft-0.8.2b1/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b1/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/action_graph.py` & `syft-0.8.2b1/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b1/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/action_object.py` & `syft-0.8.2b1/src/syft/service/action/action_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,19 +132,19 @@
         def repr_uid(_id):
             return f"{str(_id)[:3]}..{str(_id)[-1]}"
 
         arg_repr = ", ".join([repr_uid(x) for x in self.args])
         kwargs_repr = ", ".join(
             [f"{key}={repr_uid(value)}" for key, value in self.kwargs.items()]
         )
-        self_repr = (
+        _coll_repr_ = (
             f"[{repr_uid(self.remote_self)}]" if self.remote_self is not None else ""
         )
         return (
-            f"ActionObject {self.path}{self_repr}.{self.op}({arg_repr},{kwargs_repr})"
+            f"ActionObject {self.path}{_coll_repr_}.{self.op}({arg_repr},{kwargs_repr})"
         )
 
 
 class ActionObjectPointer:
     pass
 
 
@@ -403,14 +403,15 @@
     "is_pointer",
     "request",
     "__repr__",
     "_repr_markdown_",
     "syft_twin_type",
     "_repr_debug_",
     "as_empty",
+    "get",
 ]
 
 
 class ActionObject(SyftObject):
     """Action object for remote execution."""
 
     __canonical_name__ = "ActionObject"
@@ -471,15 +472,14 @@
         raise SyftException(
             f"Must init {cls} with {cls.syft_internal_type} not {type(v)}"
         )
 
     def syft_point_to(self, node_uid: UID) -> "ActionObject":
         """Set the syft_node_uid, used in the post hooks"""
         self.syft_node_uid = node_uid
-
         return self
 
     def syft_get_property(self, obj: Any, method: str) -> Any:
         klass_method = getattr(type(obj), method, None)
         if klass_method is None:
             raise Exception(f"{type(obj)} has no {method} attribute")
         return klass_method.__get__(obj)
@@ -714,25 +714,43 @@
         ) -> Action:
             return self.syft_make_action_with_self(op=op, args=args, kwargs=kwargs)
 
         return wrapper
 
     def send(self, client: SyftClient) -> Self:
         """Send the object to a Syft Client"""
-
-        return client.api.services.action.set(self)
+        res = client.api.services.action.set(self)
+        res.syft_node_location = client.id
+        res.syft_client_verify_key = client.verify_key
+        return res
 
     def get_from(self, client: SyftClient) -> Any:
         """Get the object from a Syft Client"""
         res = client.api.services.action.get(self.id)
         if not isinstance(res, ActionObject):
             return Err(res)
         else:
             return res.syft_action_data
 
+    def get(self) -> Any:
+        """Get the object from a Syft Client"""
+        # relative
+        from ...client.api import APIRegistry
+
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        res = api.services.action.get(self.id)
+
+        if not isinstance(res, ActionObject):
+            return Err(res)
+        else:
+            return res.syft_action_data
+
     def as_empty(self):
         id = self.id
         # TODO: fix
         if isinstance(id, LineageID):
             id = id.id
         return ActionObject.empty(self.syft_internal_type, id, self.syft_lineage_id)
```

### Comparing `syft-0.8.1b9/src/syft/service/action/action_permissions.py` & `syft-0.8.2b1/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/action_service.py` & `syft-0.8.2b1/src/syft/service/action/action_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             private_args = filter_twin_args(args, twin_mode=TwinMode.PRIVATE)
             private_val = private_args[0]
             setattr(resolved_self.private.syft_action_data, name, private_val)
             # todo: what do we use as data for the mock here?
             # depending on permisisons?
             public_args = filter_twin_args(args, twin_mode=TwinMode.MOCK)
             public_val = public_args[0]
-            setattr(resolved_self.mock.syft_action_data, name, public_val)
+            setattr(resolved_self.mock, name, public_val)
             return Ok(
                 TwinObject(
                     id=action.result_id,
                     private_obj=ActionObject.from_obj(
                         resolved_self.private.syft_action_data
                     ),
                     private_obj_id=action.result_id,
```

### Comparing `syft-0.8.1b9/src/syft/service/action/action_store.py` & `syft-0.8.2b1/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/action_types.py` & `syft-0.8.2b1/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/numpy.py` & `syft-0.8.2b1/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/pandas.py` & `syft-0.8.2b1/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/plan.py` & `syft-0.8.2b1/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/action/verification.py` & `syft-0.8.2b1/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/code/user_code.py` & `syft-0.8.2b1/src/syft/service/code/user_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # stdlib
 import ast
 from enum import Enum
 import hashlib
 import inspect
 from io import StringIO
+import itertools
 import sys
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
@@ -33,19 +34,22 @@
 from ...types.syft_object import SyftHashableObject
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
+from ...util.markdown import CodeMarkdown
+from ...util.markdown import as_markdown_code
 from ..context import AuthedServiceContext
 from ..dataset.dataset import Asset
 from ..metadata.node_metadata import EnclaveMetadata
 from ..policy.policy import CustomInputPolicy
 from ..policy.policy import CustomOutputPolicy
+from ..policy.policy import ExactMatch
 from ..policy.policy import InputPolicy
 from ..policy.policy import OutputPolicy
 from ..policy.policy import Policy
 from ..policy.policy import SingleExecutionExactOutput
 from ..policy.policy import SubmitUserPolicy
 from ..policy.policy import UserPolicy
 from ..policy.policy import init_policy
@@ -102,14 +106,20 @@
 
     def __init__(self, base_dict: Dict):
         self.base_dict = base_dict
 
     def __repr__(self):
         return str(self.base_dict)
 
+    def __repr_syft_nested__(self):
+        string = ""
+        for node_view, status in self.base_dict.items():
+            string += f"{node_view.node_name}: {status}<br>"
+        return string
+
     @property
     def approved(self) -> bool:
         # approved for this node only
         statuses = set(self.base_dict.values())
         return len(statuses) == 1 and UserCodeStatus.EXECUTE in statuses
 
     def for_context(self, context: AuthedServiceContext) -> UserCodeStatus:
@@ -179,23 +189,43 @@
     signature: inspect.Signature
     status: UserCodeStatusContext
     input_kwargs: List[str]
     enclave_metadata: Optional[EnclaveMetadata] = None
 
     __attr_searchable__ = ["user_verify_key", "status", "service_func_name"]
     __attr_unique__ = ["code_hash", "user_unique_func_name"]
-    __attr_repr_cols__ = ["status.approved", "service_func_name"]
+    __repr_attrs__ = ["status.approved", "service_func_name"]
 
     def __setattr__(self, key: str, value: Any) -> None:
         attr = getattr(type(self), key, None)
         if inspect.isdatadescriptor(attr):
             attr.fset(self, value)
         else:
             return super().__setattr__(key, value)
 
+    def _coll_repr_(self) -> Dict[str, Any]:
+        status = list(self.status.base_dict.values())[0].value
+        if status == UserCodeStatus.SUBMITTED.value:
+            badge_color = "badge-purple"
+        elif status == UserCodeStatus.EXECUTE.value:
+            badge_color = "badge-green"
+        else:
+            badge_color = "badge-red"
+        status_badge = {"value": status, "type": badge_color}
+        return {
+            "Input Policy": self.input_policy_type.__canonical_name__,
+            "Output Policy": self.output_policy_type.__canonical_name__,
+            "Function name": self.service_func_name,
+            "User verify key": {
+                "value": str(self.user_verify_key),
+                "type": "clipboard",
+            },
+            "Status": status_badge,
+        }
+
     @property
     def input_policy(self) -> Optional[InputPolicy]:
         if not self.status.approved:
             return None
 
         if len(self.input_policy_state) == 0:
             input_policy = None
@@ -297,20 +327,21 @@
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
 
-        node_view = NodeView(
-            node_name=api.node_name, verify_key=api.signing_key.verify_key
+        inputs = (
+            uids
+            for node_view, uids in self.input_policy_init_kwargs.items()
+            if node_view.node_name == api.node_name
         )
-        inputs = self.input_policy_init_kwargs[node_view]
         all_assets = []
-        for uid in inputs.values():
+        for uid in itertools.chain.from_iterable(x.values() for x in inputs):
             if isinstance(uid, UID):
                 assets = api.services.dataset.get_assets_by_action_id(uid)
                 if not isinstance(assets, list):
                     return assets
 
                 all_assets += assets
         return all_assets
@@ -321,14 +352,15 @@
 
         # 🟡 TODO: re-use the same infrastructure as the execute_byte_code function
         def wrapper(*args: Any, **kwargs: Any) -> Callable:
             try:
                 filtered_kwargs = {}
                 for k, v in kwargs.items():
                     filtered_kwargs[k] = debox_asset(v)
+                # third party
 
                 # remove the decorator
                 inner_function = ast.parse(self.raw_code).body[0]
                 inner_function.decorator_list = []
                 # compile the function
                 raw_byte_code = compile_byte_code(unparse(inner_function))
                 # load it
@@ -339,17 +371,37 @@
                 # return the results
                 return result
             except Exception as e:
                 print(f"Failed to run unsafe_function. {e}")
 
         return wrapper
 
+    def _repr_markdown_(self):
+        md = f"""class UserCode
+    id: str = {self.id}
+    status.approved: str = {self.status.approved}
+    service_func_name: str = {self.service_func_name}
+    code:
+
+{self.raw_code}"""
+        return as_markdown_code(md)
+
     @property
-    def code(self) -> str:
-        return self.raw_code
+    def code(self) -> CodeMarkdown:
+        return CodeMarkdown(self.raw_code)
+
+    def show_code_cell(self):
+        warning_message = """# WARNING: \n# Before you submit
+# change the name of the function \n# for no duplicates\n\n"""
+
+        # third party
+        from IPython import get_ipython
+
+        ip = get_ipython()
+        ip.set_next_input(warning_message + self.raw_code)
 
 
 @serializable(without=["local_function"])
 class SubmitUserCode(SyftObject):
     # version
     __canonical_name__ = "SubmitUserCode"
     __version__ = SYFT_OBJECT_VERSION_1
@@ -362,14 +414,16 @@
     input_policy_init_kwargs: Optional[Dict[Any, Any]] = {}
     output_policy_type: Union[SubmitUserPolicy, UID, Type[OutputPolicy]]
     output_policy_init_kwargs: Optional[Dict[Any, Any]] = {}
     local_function: Optional[Callable]
     input_kwargs: List[str]
     enclave_metadata: Optional[EnclaveMetadata] = None
 
+    __repr_attrs__ = ["func_name", "code"]
+
     @property
     def kwargs(self) -> List[str]:
         return self.input_policy_init_kwargs
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         # only run this on the client side
         if self.local_function:
@@ -384,20 +438,31 @@
         else:
             raise NotImplementedError
 
 
 def debox_asset(arg: Any) -> Any:
     deboxed_arg = arg
     if isinstance(deboxed_arg, Asset):
-        deboxed_arg = arg.mock
+        asset = deboxed_arg
+        if asset.has_data_permission():
+            return asset.data
+        else:
+            return asset.mock
     if hasattr(deboxed_arg, "syft_action_data"):
         deboxed_arg = deboxed_arg.syft_action_data
     return deboxed_arg
 
 
+def syft_function_single_use(*args: Any, **kwargs: Any):
+    return syft_function(
+        input_policy=ExactMatch(*args, **kwargs),
+        output_policy=SingleExecutionExactOutput(),
+    )
+
+
 def syft_function(
     input_policy: Union[InputPolicy, UID],
     output_policy: Optional[Union[OutputPolicy, UID]] = None,
 ) -> SubmitUserCode:
     if isinstance(input_policy, CustomInputPolicy):
         input_policy_type = SubmitUserPolicy.from_obj(input_policy)
     else:
@@ -408,14 +473,19 @@
 
     if isinstance(output_policy, CustomOutputPolicy):
         output_policy_type = SubmitUserPolicy.from_obj(output_policy)
     else:
         output_policy_type = type(output_policy)
 
     def decorator(f):
+        print(
+            f"Syft function '{f.__name__}' successfully created. "
+            f"To add a code request, please create a project using `project = syft.Project(...)`, "
+            f"then use command `project.create_code_request`."
+        )
         return SubmitUserCode(
             code=inspect.getsource(f),
             func_name=f.__name__,
             signature=inspect.signature(f),
             input_policy_type=input_policy_type,
             input_policy_init_kwargs=input_policy.init_kwargs,
             output_policy_type=output_policy_type,
```

### Comparing `syft-0.8.1b9/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b1/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/code/user_code_service.py` & `syft-0.8.2b1/src/syft/service/code/user_code_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             # Check if the code is approved
             if status.for_context(context) != UserCodeStatus.EXECUTE:
                 if status.for_context(context) == UserCodeStatus.SUBMITTED:
                     return SyftNotReady(
                         message=f"{type(code_item)} Your code is waiting for approval: {status}"
                     )
                 return SyftError(
-                    message=f"{type(code_item)} Your code cannot be run: {status}"
+                    message=f"{type(code_item)} Your code cannot be run: {status.for_context(context)}"
                 )
 
             output_policy = code_item.output_policy
             if output_policy is None:
                 raise Exception("Output policy not approved", code_item)
 
             # Check if the OutputPolicy is valid
```

### Comparing `syft-0.8.1b9/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b1/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/context.py` & `syft-0.8.2b1/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b1/src/syft/service/data_subject/data_subject.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,22 +43,26 @@
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
         members = api.services.data_subject.members_for(self.name)
         return members
 
     __attr_searchable__ = ["name", "description"]
+    __repr_attrs__ = ["name", "description"]
     __attr_unique__ = ["name"]
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __eq__(self, other) -> bool:
         return hash(self) == hash(other)
 
+    def __repr_syft_nested__(self):
+        return f"DataSubject({self.name})"
+
     def __repr__(self) -> str:
         return f"<DataSubject: {self.name}>"
 
     def _repr_markdown_(self) -> str:
         _repr_str = f"DataSubject: {self.name}\n"
         _repr_str += f"Description: {self.description}\n"
         _repr_str += f"Aliases: {self.aliases}\n"
@@ -76,21 +80,29 @@
     name: str
     description: Optional[str]
     aliases: Optional[List[str]] = []
     members: Dict[str, "DataSubjectCreate"] = {}
 
     __attr_searchable__ = ["name", "description"]
     __attr_unique__ = ["name"]
+    __repr_attrs__ = ["name", "member_count"]
+
+    @property
+    def member_count(self):
+        return len(self.members)
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __eq__(self, other) -> bool:
         return hash(self) == hash(other)
 
+    def __repr_syft_nested__(self):
+        return f"DataSubject({self.name})"
+
     def _create_member_relationship(self, data_subject, _relationship_set):
         for member in data_subject.members.values():
             _relationship_set.add((data_subject, member))
             self._create_member_relationship(member, _relationship_set)
 
     def add_member(self, data_subject: Self) -> None:
         self.members[data_subject.name] = data_subject
```

### Comparing `syft-0.8.1b9/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b1/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b1/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b1/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/dataset/dataset.py` & `syft-0.8.2b1/src/syft/service/dataset/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 # stdlib
 from collections import OrderedDict
 from datetime import datetime
 from enum import Enum
-import sys
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 # third party
 import itables
+import pandas as pd
 from pydantic import ValidationError
 from pydantic import root_validator
 from pydantic import validator
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import PartitionKey
 from ...types.datetime import DateTime
-from ...types.syft_object import SURFACE_DARK_BRIGHT
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
-from ...types.syft_object import itables_css
 from ...types.transforms import TransformContext
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.transforms import validate_url
 from ...types.uid import UID
+from ...util import options
+from ...util.colors import ON_SURFACE_HIGHEST
+from ...util.colors import SURFACE
+from ...util.colors import SURFACE_SURFACE
+from ...util.fonts import ITABLES_CSS
+from ...util.fonts import fonts_css
 from ...util.markdown import as_markdown_python_code
+from ...util.notebook_ui.notebook_addons import FOLDER_ICON
+from ...util.util import get_mb_size
 from ..data_subject.data_subject import DataSubject
 from ..data_subject.data_subject import DataSubjectCreate
 from ..data_subject.data_subject_service import DataSubjectService
 from ..response import SyftError
 from ..response import SyftException
 from ..response import SyftSuccess
 
+DATA_SIZE_WARNING_LIMIT = 512
+
 
 @serializable()
 class TupleDict(OrderedDict):
     def __getitem__(self, key: Union[str, int]) -> Any:
         if isinstance(key, int):
             return list(self.values())[key]
         return super(TupleDict, self).__getitem__(key)
@@ -55,20 +63,33 @@
 
 @serializable()
 class Contributor(SyftObject):
     __canonical_name__ = "Contributor"
     __version__ = SYFT_OBJECT_VERSION_1
 
     name: str
-    role: str
+    role: Optional[str]
     email: str
     phone: Optional[str]
     note: Optional[str]
 
-    __attr_repr_cols__ = ["name", "role", "email"]
+    __repr_attrs__ = ["name", "role", "email"]
+
+    def _repr_html_(self) -> Any:
+        return f"""
+            <style>
+            .syft-contributor {{color: {SURFACE[options.color_theme]};}}
+            </style>
+            <div class='syft-contributor' style="line-height:25%">
+                <h3>Contributor</h3>
+                <p><strong>Name: </strong>{self.name}</p>
+                <p><strong>Role: </strong>{self.role}</p>
+                <p><strong>Email: </strong>{self.email}</p>
+            </div>
+            """
 
 
 @serializable()
 class Asset(SyftObject):
     # version
     __canonical_name__ = "Asset"
     __version__ = SYFT_OBJECT_VERSION_1
@@ -79,56 +100,64 @@
     description: Optional[str]
     contributors: List[Contributor] = []
     data_subjects: List[DataSubject] = []
     mock_is_real: bool = False
     shape: Optional[Tuple]
     created_at: DateTime = DateTime.now()
 
-    __attr_repr_cols__ = ["name", "shape"]
-
-    # @property
-    # def pointer(self) -> ActionObjectPointer:
-    #     api = APIRegistry.api_for(node_uid=self.node_uid)
-    #     obj_ptr = api.services.action.get_pointer(uid=self.action_id)
-    #     return obj_ptr
+    __repr_attrs__ = ["name", "shape"]
 
     def _repr_html_(self) -> Any:
+        itables_css = f"""
+        .itables table {{
+            margin: 0 auto;
+            float: left;
+            color: {ON_SURFACE_HIGHEST[options.color_theme]};
+        }}
+        .itables table th {{color: {SURFACE_SURFACE[options.color_theme]};}}
+        """
+
         # relative
         from ...service.action.action_object import ActionObject
 
-        uploaded_by_line = ""
+        uploaded_by_line = "n/a"
         if len(self.contributors) > 0:
             uploaded_by_line = (
                 f"<p><strong>Uploaded by: </strong>{self.contributors[0].name}</p>"
             )
         if isinstance(self.data, ActionObject):
             data_table_line = itables.to_html_datatable(
                 df=self.data.syft_action_data, css=itables_css
             )
+        elif isinstance(self.data, pd.DataFrame):
+            data_table_line = itables.to_html_datatable(df=self.data, css=itables_css)
         else:
             data_table_line = self.data
-        return (
-            f"""
+        return f"""
             <style>
-            .syft-asset {{color: {SURFACE_DARK_BRIGHT};}}
+            {fonts_css}
+            .syft-asset {{color: {SURFACE[options.color_theme]};}}
+            .syft-asset h3,
+            .syft-asset p
+              {{font-family: 'Open Sans'}}
+            {ITABLES_CSS}
             </style>
-            """
-            + '<div class="syft-asset">'
-            + f"<h3>{self.name}</h3>"
-            + f"<p>{self.description}</p>"
-            + f"<p><strong>Asset ID: </strong>{self.id}</p>"
-            + f"<p><strong>Action Object ID: </strong>{self.action_id}</p>"
-            + uploaded_by_line
-            + f"<p><strong>Created on: </strong>{self.created_at}</p>"
-            + "<p><strong>Data:</strong></p>"
-            + data_table_line
-            + "<p><strong>Mock Data:</strong></p>"
-            + itables.to_html_datatable(df=self.mock_data, css=itables_css)
-            + "</div>"
-        )
+
+            <div class="syft-asset">
+            <h3>{self.name}</h3>
+            <p>{self.description}</p>
+            <p><strong>Asset ID: </strong>{self.id}</p>
+            <p><strong>Action Object ID: </strong>{self.action_id}</p>
+            {uploaded_by_line}
+            <p><strong>Created on: </strong>{self.created_at}</p>
+            <p><strong>Data:</strong></p>
+            {data_table_line}
+            <p><strong>Mock Data:</strong></p>
+            {itables.to_html_datatable(df=self.mock, css=itables_css)}
+            </div>"""
 
     def _repr_markdown_(self) -> str:
         _repr_str = f"Asset: {self.name}\n"
         _repr_str += f"Pointer Id: {self.action_id}\n"
         _repr_str += f"Description: {self.description}\n"
         _repr_str += f"Total Data Subjects: {len(self.data_subjects)}\n"
         _repr_str += f"Shape: {self.shape}\n"
@@ -145,45 +174,49 @@
         api = APIRegistry.api_for(
             node_uid=self.node_uid,
             user_verify_key=self.syft_client_verify_key,
         )
         return api.services.action.get_pointer(self.action_id)
 
     @property
-    def mock_data(self) -> Any:
+    def mock(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(
             node_uid=self.node_uid,
             user_verify_key=self.syft_client_verify_key,
         )
         return api.services.action.get_pointer(self.action_id).syft_action_data
 
-    @property
-    def mock(self) -> Any:
-        # relative
-        from ...client.api import APIRegistry
+    def has_data_permission(self):
+        return self.data is not None
 
-        api = APIRegistry.api_for(
-            node_uid=self.node_uid,
-            user_verify_key=self.syft_client_verify_key,
+    def has_permission(self, data_result):
+        # TODO: implement in a better way
+        return not (
+            isinstance(data_result, str)
+            and data_result.startswith("Permission")
+            and data_result.endswith("denied")
         )
-        return api.services.action.get_pointer(self.action_id)
 
     @property
     def data(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(
             node_uid=self.node_uid,
             user_verify_key=self.syft_client_verify_key,
         )
-        return api.services.action.get(self.action_id)
+        res = api.services.action.get(self.action_id)
+        if self.has_permission(res):
+            return res.syft_action_data
+        else:
+            return None
 
 
 def _is_action_data_empty(obj: Any) -> bool:
     # just a wrapper of action_object.is_action_data_empty
     # to work around circular import error
 
     # relative
@@ -214,14 +247,16 @@
     action_id: Optional[UID]
     data: Optional[Any]
     mock: Optional[Any]
     shape: Optional[Tuple]
     mock_is_real: bool = False
     created_at: Optional[DateTime]
 
+    __repr_attrs__ = ["name"]
+
     class Config:
         validate_assignment = True
 
     @root_validator()
     def __empty_mock_cannot_be_real(cls, values: dict[str, Any]) -> Dict:
         """set mock_is_real to False whenever mock is None or empty"""
 
@@ -242,23 +277,29 @@
     def add_data_subject(self, data_subject: DataSubject) -> None:
         self.data_subjects.append(data_subject)
 
     def add_contributor(
         self,
         name: str,
         email: str,
-        role: Union[Enum, str],
+        role: Optional[Union[Enum, str]] = None,
         phone: Optional[str] = None,
         note: Optional[str] = None,
-    ) -> None:
-        _role_str = role.value if isinstance(role, Enum) else role
-        contributor = Contributor(
-            name=name, role=_role_str, email=email, phone=phone, note=note
-        )
-        self.contributors.append(contributor)
+    ) -> Union[SyftSuccess, SyftError]:
+        try:
+            _role_str = role.value if isinstance(role, Enum) else role
+            contributor = Contributor(
+                name=name, role=_role_str, email=email, phone=phone, note=note
+            )
+            self.contributors.append(contributor)
+            return SyftSuccess(
+                message=f"Contributor '{name}' added to '{self.name}' Asset."
+            )
+        except Exception as e:
+            return SyftError(message=f"Failed to add contributor. Error: {e}")
 
     def set_description(self, description: str) -> None:
         self.description = description
 
     def set_obj(self, data: Any) -> None:
         if isinstance(data, SyftError):
             raise SyftException(data)
@@ -294,14 +335,21 @@
         if not _is_action_data_empty(self.mock):
             data_shape = get_shape_or_len(self.data)
             mock_shape = get_shape_or_len(self.mock)
             if data_shape != mock_shape:
                 return SyftError(
                     message=f"set_obj shape {data_shape} must match set_mock shape {mock_shape}"
                 )
+        total_size_mb = get_mb_size(self.data) + get_mb_size(self.mock)
+        if total_size_mb > DATA_SIZE_WARNING_LIMIT:
+            print(
+                f"**WARNING**: The total size for asset: '{self.name}' exceeds '{DATA_SIZE_WARNING_LIMIT} MB'. "
+                "This might result in failure to upload dataset. "
+                "Please contact #support on OpenMined slack for further assistance.",
+            )
 
         return SyftSuccess(message="Dataset is Valid")
 
 
 def get_shape_or_len(obj: Any) -> Optional[Union[Tuple[int, ...], int]]:
     if hasattr(obj, "shape"):
         shape = getattr(obj, "shape", None)
@@ -330,38 +378,56 @@
     updated_at: Optional[str]
     requests: Optional[int] = 0
     mb_size: Optional[int]
     created_at: DateTime = DateTime.now()
 
     __attr_searchable__ = ["name", "citation", "url", "description", "action_ids"]
     __attr_unique__ = ["name"]
-    __attr_repr_cols__ = ["name", "url"]
+    __repr_attrs__ = ["name", "url", "created_at"]
+
+    @property
+    def icon(self):
+        return FOLDER_ICON
+
+    def _coll_repr_(self) -> Dict[str, Any]:
+        return {
+            "Name": self.name,
+            "Assets": len(self.asset_list),
+            "Size": f"{self.mb_size} (MB)",
+            "Url": self.url,
+            "created at": str(self.created_at),
+        }
 
     def _repr_html_(self) -> Any:
-        uploaded_by_line = ""
+        uploaded_by_line = "n/a"
         if len(self.contributors) > 0:
             uploaded_by_line = (
-                f"<p><strong>Uploaded by: </strong>{self.contributors[0].name}</p>"
+                "<p class='paragraph-sm'><strong>"
+                + f"<span class='pr-8'>Uploaded by:</span></strong>{self.contributors[0].name}</p>"
             )
-        return (
-            f"""
+        return f"""
             <style>
-            .syft-dataset {{color: {SURFACE_DARK_BRIGHT};}}
+            {fonts_css}
+            .syft-dataset {{color: {SURFACE[options.color_theme]};}}
+            .syft-dataset h3,
+            .syft-dataset p
+              {{font-family: 'Open Sans';}}
+              {ITABLES_CSS}
             </style>
+            <div class='syft-dataset'>
+            <h3>{self.name}</h3>
+            <p>{self.description}</p>
+            {uploaded_by_line}
+            <p class='paragraph-sm'><strong><span class='pr-8'>Created on: </span></strong>{self.created_at}</p>
+            <p class='paragraph-sm'><strong><span class='pr-8'>URL:
+            </span></strong><a href='{self.url}'>{self.url}</a></p>
+            <p class='paragraph-sm'><strong><span class='pr-8'>Contributors:</span></strong>
+            to see full details call <strong>dataset.contributors</strong></p>
+            {self.assets._repr_html_()}
             """
-            + "<div class='syft-dataset'>"
-            + f"<h3>{self.name}</h3>"
-            + f"<p>{self.description}</p>"
-            + uploaded_by_line
-            + f"<p><strong>Created on: </strong>{self.created_at}</p>"
-            + f'<p><strong>URL: </strong><a href="{self.url}">{self.url}</a></p>'
-            + "<p><strong>Contributors: </strong> to see full details call dataset.contributors</p>"
-            + self.asset_list._repr_html_()
-            + "</div>"
-        )
 
     def action_ids(self) -> List[UID]:
         data = []
         for asset in self.asset_list:
             if asset.action_id:
                 data.append(asset.action_id)
         return data
@@ -445,14 +511,16 @@
 @serializable()
 class CreateDataset(Dataset):
     # version
     __canonical_name__ = "CreateDataset"
     __version__ = SYFT_OBJECT_VERSION_1
     asset_list: List[CreateAsset] = []
 
+    __repr_attrs__ = ["name", "url"]
+
     id: Optional[UID] = None
     created_at: Optional[DateTime]
 
     class Config:
         validate_assignment = True
 
     def _check_asset_must_contain_mock(self) -> None:
@@ -474,40 +542,68 @@
     def add_url(self, url: str) -> None:
         self.url = url
 
     def add_contributor(
         self,
         name: str,
         email: str,
-        role: Union[Enum, str],
+        role: Optional[Union[Enum, str]] = None,
         phone: Optional[str] = None,
         note: Optional[str] = None,
-    ) -> None:
-        _role_str = role.value if isinstance(role, Enum) else role
-        contributor = Contributor(
-            name=name, role=_role_str, email=email, phone=phone, note=note
-        )
-        self.contributors.append(contributor)
+    ) -> Union[SyftSuccess, SyftError]:
+        try:
+            _role_str = role.value if isinstance(role, Enum) else role
+            contributor = Contributor(
+                name=name, role=_role_str, email=email, phone=phone, note=note
+            )
+            self.contributors.append(contributor)
+            return SyftSuccess(
+                message=f"Contributor '{name}' added to '{self.name}' Dataset."
+            )
+        except Exception as e:
+            return SyftError(message=f"Failed to add contributor. Error: {e}")
 
-    def add_asset(self, asset: CreateAsset) -> None:
+    def add_asset(
+        self, asset: CreateAsset, force_replace=False
+    ) -> Union[SyftSuccess, SyftError]:
         if asset.mock is None:
             raise ValueError(_ASSET_WITH_NONE_MOCK_ERROR_MESSAGE)
 
+        for i, existing_asset in enumerate(self.asset_list):
+            if existing_asset.name == asset.name:
+                if not force_replace:
+                    return SyftError(
+                        message=f"""Asset "{asset.name}" already exists in '{self.name}' Dataset."""
+                        """ Use add_asset(asset, force_replace=True) to replace."""
+                    )
+                else:
+                    self.asset_list[i] = asset
+                    return SyftSuccess(
+                        f"Asset {asset.name} has been successfully replaced."
+                    )
+
         self.asset_list.append(asset)
 
+        return SyftSuccess(
+            message=f"Asset '{asset.name}' added to '{self.name}' Dataset."
+        )
+
     def remove_asset(self, name: str) -> None:
         asset_to_remove = None
         for asset in self.asset_list:
             if asset.name == name:
                 asset_to_remove = asset
                 break
 
         if asset_to_remove is None:
-            print(f"No asset exists with name: {name}")
+            return SyftError(message=f"No asset exists with name: {name}")
         self.asset_list.remove(asset_to_remove)
+        return SyftSuccess(
+            message=f"Asset '{self.name}' removed from '{self.name}' Dataset."
+        )
 
     def check(self) -> Result[SyftSuccess, List[SyftError]]:
         errors = []
         for asset in self.asset_list:
             result = asset.check()
             if not result:
                 errors.append(result)
@@ -580,21 +676,18 @@
         create_and_store_twin,
         set_data_subjects,
     ]
 
 
 def convert_asset(context: TransformContext) -> TransformContext:
     assets = context.output.pop("asset_list", [])
-    dataset_size = 0
     for idx, create_asset in enumerate(assets):
-        dataset_size += sys.getsizeof(assets) / 1024
         asset_context = TransformContext.from_context(obj=create_asset, context=context)
         assets[idx] = create_asset.to(Asset, context=asset_context)
     context.output["asset_list"] = assets
-    context.output["mb_size"] = dataset_size
     return context
 
 
 def add_current_date(context: TransformContext) -> TransformContext:
     current_date = datetime.now()
     formatted_date = current_date.strftime("%b %d, %Y")
     context.output["updated_at"] = formatted_date
```

### Comparing `syft-0.8.1b9/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b1/src/syft/service/dataset/dataset_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import DATA_OWNER_ROLE_LEVEL
+from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .dataset import Asset
 from .dataset import CreateDataset
 from .dataset import Dataset
 from .dataset_stash import DatasetStash
 
 
@@ -48,15 +49,18 @@
                 ActionObjectPermission(
                     uid=dataset.id, permission=ActionPermission.ALL_READ
                 ),
             ],
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
-        return SyftSuccess(message="Dataset Added")
+        return SyftSuccess(
+            message=f"Dataset uploaded to '{context.node.name}'. "
+            f"To see the datasets uploaded by a client on this node, use command `[your_client].datasets`"
+        )
 
     @service_method(path="dataset.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(
         self,
         context: AuthedServiceContext,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
@@ -130,15 +134,17 @@
             datasets = result.ok()
             for dataset in datasets:
                 dataset.node_uid = context.node.id
             return datasets
         return SyftError(message=result.err())
 
     @service_method(
-        path="dataset.get_assets_by_action_id", name="get_assets_by_action_id"
+        path="dataset.get_assets_by_action_id",
+        name="get_assets_by_action_id",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def get_assets_by_action_id(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[List[Asset], SyftError]:
         """Get Assets by an Action ID"""
         datasets = self.get_by_action_id(context=context, uid=uid)
         assets = []
```

### Comparing `syft-0.8.1b9/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b1/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/message/message_service.py` & `syft-0.8.2b1/src/syft/service/message/message_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Union
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectREAD
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
@@ -37,15 +38,25 @@
     @service_method(path="messages.send", name="send")
     def send(
         self, context: AuthedServiceContext, message: CreateMessage
     ) -> Union[Message, SyftError]:
         """Send a new message"""
 
         new_message = message.to(Message, context=context)
-        result = self.stash.set(context.credentials, new_message)
+
+        # Add read permissions to person receiving this message
+        permissions = [
+            ActionObjectREAD(
+                uid=new_message.id, credentials=new_message.to_user_verify_key
+            )
+        ]
+
+        result = self.stash.set(
+            context.credentials, new_message, add_permissions=permissions
+        )
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(path="messages.reply", name="reply", roles=GUEST_ROLE_LEVEL)
     def reply(
         self,
@@ -65,18 +76,23 @@
             else:
                 SyftError(
                     message="Couldn't add a new message reply in the target message."
                 )
         else:
             SyftError(message="The target message id {reply.target_msg} was not found!")
 
-    @service_method(path="messages.get_all", name="get_all")
+    @service_method(
+        path="messages.get_all",
+        name="get_all",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
+    )
     def get_all(self, context: AuthedServiceContext) -> Union[List[Message], SyftError]:
         result = self.stash.get_all_inbox_for_verify_key(
-            context.credentials, verify_key=context.credentials
+            credentials=context.credentials,
+            verify_key=context.credentials,
         )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
     @service_method(
@@ -105,25 +121,33 @@
             context.credentials, verify_key=context.credentials, status=status
         )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
-    @service_method(path="messages.get_all_read", name="get_all_read")
+    @service_method(
+        path="messages.get_all_read",
+        name="get_all_read",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
+    )
     def get_all_read(
         self,
         context: AuthedServiceContext,
     ) -> Union[List[Message], SyftError]:
         return self.get_all_for_status(
             context=context,
             status=MessageStatus.READ,
         )
 
-    @service_method(path="messages.get_all_unread", name="get_all_unread")
+    @service_method(
+        path="messages.get_all_unread",
+        name="get_all_unread",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
+    )
     def get_all_unread(
         self,
         context: AuthedServiceContext,
     ) -> Union[List[Message], SyftError]:
         return self.get_all_for_status(
             context=context,
             status=MessageStatus.UNREAD,
```

### Comparing `syft-0.8.1b9/src/syft/service/message/message_stash.py` & `syft-0.8.2b1/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/message/messages.py` & `syft-0.8.2b1/src/syft/service/message/messages.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,22 +56,30 @@
     replies: Optional[List[ReplyMessage]] = []
 
     __attr_searchable__ = [
         "from_user_verify_key",
         "to_user_verify_key",
         "status",
     ]
-    __attr_repr_cols__ = ["subject", "status", "created_at", "linked_obj"]
+    __repr_attrs__ = ["subject", "status", "created_at", "linked_obj"]
 
     @property
     def link(self) -> Optional[SyftObject]:
         if self.linked_obj:
             return self.linked_obj.resolve
         return None
 
+    def _coll_repr_(self):
+        return {
+            "Subject": self.subject,
+            "Status": self.status.name.capitalize(),
+            "Created At": str(self.created_at),
+            "Linked object": f"{self.linked_obj.object_type.__canonical_name__} ({self.linked_obj.object_uid})",
+        }
+
     def mark_read(self) -> None:
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         return api.services.messages.mark_as_read(uid=self.id)
 
     def mark_unread(self) -> None:
         api = APIRegistry.api_for(
             self.node_uid,
```

### Comparing `syft-0.8.1b9/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b1/src/syft/service/metadata/node_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     lowest_object_version: int
     syft_version: str
     node_type: str = "Domain"
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "Text"
+    signup_enabled: bool
 
     def check_version(self, client_version: str) -> None:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
@@ -92,14 +93,15 @@
     lowest_object_version: int
     syft_version: str
     node_type: str = "Domain"
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "My cool domain"
+    signup_enabled: bool
 
     def check_version(self, client_version: str) -> bool:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
```

### Comparing `syft-0.8.1b9/src/syft/service/network/network_service.py` & `syft-0.8.2b1/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/network/node_peer.py` & `syft-0.8.2b1/src/syft/service/network/node_peer.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     verify_key: SyftVerifyKey
     is_vpn: bool = False
     vpn_auth_key: Optional[str] = None
     node_routes: List[NodeRoute] = []
 
     __attr_searchable__ = ["name"]
     __attr_unique__ = ["verify_key"]
-    __attr_repr_cols__ = ["name"]
+    __repr_attrs__ = ["name"]
 
     def update_routes(self, new_routes: List[NodeRoute]) -> None:
         add_routes = []
         existing_routes = set(self.node_routes)
         for new_route in new_routes:
             if new_route not in existing_routes:
                 add_routes.append(new_route)
```

### Comparing `syft-0.8.1b9/src/syft/service/network/routes.py` & `syft-0.8.2b1/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/policy/policy.py` & `syft-0.8.2b1/src/syft/service/policy/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     __version__ = SYFT_OBJECT_VERSION_1
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         if "init_kwargs" in kwargs:
             init_kwargs = kwargs["init_kwargs"]
             del kwargs["init_kwargs"]
         else:
-            # TODO: remove this tech debt
+            # TODO: remove this tech debt, dont remove the id mapping functionality
             init_kwargs = partition_by_node(kwargs)
         super().__init__(*args, init_kwargs=init_kwargs, **kwargs)
 
     def filter_kwargs(
         self, kwargs: Dict[Any, Any], context: AuthedServiceContext, code_item_id: UID
     ) -> Dict[Any, Any]:
         raise NotImplementedError
```

### Comparing `syft-0.8.1b9/src/syft/service/policy/policy_service.py` & `syft-0.8.2b1/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b1/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/project/project.py` & `syft-0.8.2b1/src/syft/service/project/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,23 @@
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...service.metadata.node_metadata import NodeMetadata
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
+from ...types.syft_object import short_qual_name
 from ...types.transforms import TransformContext
 from ...types.transforms import keep
 from ...types.transforms import transform
 from ...types.uid import UID
+from ...util import options
+from ...util.colors import SURFACE
 from ...util.markdown import markdown_as_class_with_fields
+from ...util.util import full_name_with_qualname
 from ..code.user_code import SubmitUserCode
 from ..network.network_service import NodePeer
 from ..network.routes import NodeRoute
 from ..network.routes import connection_to_route
 from ..request.request import Request
 from ..response import SyftError
 from ..response import SyftException
@@ -59,15 +63,15 @@
 class Identity(SyftObject):
     __canonical_name__ = "Identity"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
     verify_key: SyftVerifyKey
 
-    __attr_repr_cols__ = ["id", "verify_key"]
+    __repr_attrs__ = ["id", "verify_key"]
 
     def __repr__(self) -> str:
         verify_key_str = f"{self.verify_key}"
         return f"<🔑 {verify_key_str[0:8]} @ 🟢 {self.id.short()}>"
 
     @classmethod
     def from_client(cls, client: SyftClient) -> Identity:
@@ -112,14 +116,20 @@
     prev_event_uid: Optional[UID]
     prev_event_hash: Optional[str]
     event_hash: Optional[str]
     # 3. Signature attrs
     creator_verify_key: Optional[SyftVerifyKey]
     signature: Optional[bytes]  # dont use in signing
 
+    def __repr_syft_nested__(self):
+        return (
+            short_qual_name(full_name_with_qualname(self)),
+            f"{str(self.id)[:4]}...{str(self.id)[-3:]}",
+        )
+
     @pydantic.root_validator(pre=True)
     def make_timestamp(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "timestamp" not in values or values["timestamp"] is None:
             values["timestamp"] = DateTime.now()
         return values
 
     def _pre_add_update(self, project: Project) -> None:
@@ -301,15 +311,15 @@
                 f"linked_request should be either Request or LinkedObject, got {type(v)}"
             )
 
     @property
     def request(self):
         return self.linked_request.resolve
 
-    __attr_repr_cols__ = [
+    __repr_attrs__ = [
         "request.status",
         "request.changes[-1].link.service_func_name",
     ]
 
     def _repr_markdown_(self) -> str:
         func_name = None
         if len(self.request.changes) > 0:
@@ -628,15 +638,15 @@
 
 
 def add_code_request_to_project(
     project: Union[ProjectSubmit, Project],
     code: SubmitUserCode,
     client: SyftClient,
     reason: Optional[str] = None,
-):
+) -> Union[SyftError, SyftSuccess]:
     if not isinstance(code, SubmitUserCode):
         return SyftError(
             message=f"Currently we are  only support creating requests for SubmitUserCode: {type(code)}"
         )
 
     if not isinstance(client, SyftClient):
         return SyftError(message="Client should be a valid SyftClient")
@@ -655,23 +665,26 @@
     if isinstance(project, ProjectSubmit):
         project.bootstrap_events.append(request_event)
     else:
         result = project.add_event(request_event)
         if isinstance(result, SyftError):
             return result
 
-    return SyftSuccess(message="Request added successfully")
+    return SyftSuccess(
+        message=f"Code request for '{code.func_name}' successfully added to '{project.name}' Project. "
+        f"To see code requests by a client, run `[your_client].code`"
+    )
 
 
 @serializable()
 class Project(SyftObject):
     __canonical_name__ = "Project"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    __attr_repr_cols__ = ["name", "description", "created_by", "events"]
+    __repr_attrs__ = ["name", "description", "created_by"]
     __attr_unique__ = ["name"]
 
     # TODO: re-add users, members, leader_node_peer
     __hash_exclude_attrs__ = [
         "user_signing_key",
         "start_hash",
         "users",
@@ -700,14 +713,37 @@
 
     # Unused
     consensus_model: ConsensusModel
     project_permissions: Set[str]
     # store: Dict[UID, Dict[UID, SyftObject]] = {}
     # permissions: Dict[UID, Dict[UID, Set[str]]] = {}
 
+    def _coll_repr_(self):
+        return {
+            "Name": self.name,
+            "description": self.description,
+            "created by": self.created_by,
+        }
+
+    def _repr_html_(self) -> Any:
+        return (
+            f"""
+            <style>
+            .syft-project {{color: {SURFACE[options.color_theme]};}}
+            </style>
+            """
+            + "<div class='syft-project'>"
+            + f"<h3>{self.name}</h3>"
+            + f"<p>{self.description}</p>"
+            + f"<p><strong>Created by: </strong>{self.created_by}</p>"
+            + self.requests._repr_html_()
+            + "<p>To see a list of projects, use command `&lt;your_client&gt;.projects`</p>"
+            + "</div>"
+        )
+
     def _broadcast_event(
         self, project_event: ProjectEvent
     ) -> Union[SyftSuccess, SyftError]:
         leader_client = self.get_leader_client(self.user_signing_key)
 
         return leader_client.api.services.project.broadcast_event(project_event)
 
@@ -779,16 +815,17 @@
             # Retrying broadcasting the event to leader
             # recursively call _append_event as due to network latency the event could reach late
             # and other events would be being streamed to the leader
             # This scenario could lead to starvation of node trying to sync with the leader
             # This would be solved in our future leaderless approach
             return self._append_event(event=event, credentials=credentials)
 
-        self.events.append(copy.deepcopy(event))
-        self.event_id_hashmap[event.id] = event
+        event_copy = copy.deepcopy(event)
+        self.events.append(event_copy)
+        self.event_id_hashmap[event.id] = event_copy
         return result
 
     @property
     def event_ids(self) -> Iterable[UID]:
         return self.event_id_hashmap.keys()
 
     def add_event(
@@ -1116,15 +1153,15 @@
         "members",
         "clients",
         "leader_node_route",
         "bootstrap_events",
     ]
 
     # stash rules
-    __attr_repr_cols__ = ["name", "description", "created_by"]
+    __repr_attrs__ = ["name", "description", "created_by"]
     __attr_unique__ = ["name"]
 
     id: UID
 
     # Init args
     name: str
     description: Optional[str]
@@ -1161,14 +1198,28 @@
 
         # Extract information of logged in user from syft clients
         self.users = [UserIdentity.from_client(client) for client in self.clients]
 
         # Convert SyftClients to NodeIdentities
         self.members = list(map(self.to_node_identity, self.members))
 
+    def _repr_html_(self) -> Any:
+        return (
+            f"""
+            <style>
+            .syft-project-create {{color: {SURFACE[options.color_theme]};}}
+            </style>
+            """
+            + "<div class='syft-project-create'>"
+            + f"<h3>{self.name}</h3>"
+            + f"<p>{self.description}</p>"
+            + f"<p><strong>Created by: </strong>{self.created_by}</p>"
+            + "</div>"
+        )
+
     @validator("members", pre=True)
     def verify_members(cls, val: Union[List[SyftClient], List[NodeIdentity]]):
         # SyftClients must be logged in by the same emails
         clients = cls.get_syft_clients(val)
         if len(clients) > 0:
             emails = set([client.logged_in_user for client in clients])
             if len(emails) > 1:
@@ -1347,15 +1398,15 @@
         ]
     )
 
 
 def create_project_event_hash(project_event: ProjectEvent) -> Tuple[bytes, str]:
     # Creating a custom hash for the project
     # as the recursive hash is yet to be revamped
-    # for primitives python types
+    # for primitives python types.
 
     # hashing is calculated based on the following attributes
     # attrs = ["id", "project_id", "seq no",
     #  "prev_event_uid", "prev_event_hash", "creator_verify_key"]
 
     return hash_object(
         [
```

### Comparing `syft-0.8.1b9/src/syft/service/project/project_service.py` & `syft-0.8.2b1/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/project/project_stash.py` & `syft-0.8.2b1/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/queue/base_queue.py` & `syft-0.8.2b1/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/queue/queue.py` & `syft-0.8.2b1/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b1/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b1/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/request/request.py` & `syft-0.8.2b1/src/syft/service/request/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # stdlib
 from enum import Enum
 import hashlib
 import inspect
 from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 # third party
 from result import Err
@@ -27,15 +28,18 @@
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import LineageID
 from ...types.uid import UID
+from ...util import options
+from ...util.colors import SURFACE
 from ...util.markdown import markdown_as_class_with_fields
+from ...util.notebook_ui.notebook_addons import REQUEST_ICON
 from ..action.action_object import ActionObject
 from ..action.action_service import ActionService
 from ..action.action_store import ActionObjectPermission
 from ..action.action_store import ActionPermission
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatus
 from ..context import AuthedServiceContext
@@ -82,15 +86,15 @@
 class ActionStoreChange(Change):
     __canonical_name__ = "ActionStoreChange"
     __version__ = SYFT_OBJECT_VERSION_1
 
     linked_obj: LinkedObject
     apply_permission_type: ActionPermission
 
-    __attr_repr_cols__ = ["linked_obj", "apply_permission_type"]
+    __repr_attrs__ = ["linked_obj", "apply_permission_type"]
 
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             action_service = context.node.get_service(ActionService)
             action_store = action_service.store
@@ -109,72 +113,147 @@
                     uid=obj_uid,
                     credentials=context.requesting_user_credentials,
                     permission=self.apply_permission_type,
                 )
                 if apply:
                     action_store.add_permission(requesting_permission)
                 else:
-                    action_store.remove_permission(requesting_permission)
+                    if action_store.has_permission(requesting_permission):
+                        action_store.remove_permission(requesting_permission)
             else:
                 return Err(
                     SyftError(
                         message=f"No permission for approving_user_credentials {context.approving_user_credentials}"
                     )
                 )
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}")
             return Err(SyftError(message=str(e)))
 
     def apply(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=True)
 
-    def revert(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
+    def undo(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=False)
 
+    def __repr_syft_nested__(self):
+        return f"Apply <b>{self.apply_permission_type}</b> to \
+            <i>{self.linked_obj.object_type.__canonical_name__}:{self.linked_obj.object_uid.short()}</i>"
+
 
 @serializable()
 class Request(SyftObject):
     __canonical_name__ = "Request"
     __version__ = SYFT_OBJECT_VERSION_1
 
     requesting_user_verify_key: SyftVerifyKey
+    requesting_user_name: str
     approving_user_verify_key: Optional[SyftVerifyKey]
     request_time: DateTime
-    approval_time: Optional[DateTime]
+    updated_at: Optional[DateTime]
     node_uid: UID
     request_hash: str
     changes: List[Change]
     history: List[ChangeStatus] = []
 
     __attr_searchable__ = [
         "requesting_user_verify_key",
         "approving_user_verify_key",
     ]
     __attr_unique__ = ["request_hash"]
-    __attr_repr_cols__ = [
+    __repr_attrs__ = [
         "request_time",
-        "approval_time",
+        "updated_at",
         "status",
         "changes",
         "requesting_user_verify_key",
     ]
 
+    def _repr_html_(self) -> Any:
+        # add changes
+        updated_at_line = ""
+        if self.updated_at is not None:
+            updated_at_line += (
+                f"<p><strong>Created by: </strong>{self.requesting_user_name}</p>"
+            )
+        str_changes = []
+        for change in self.changes:
+            str_change = (
+                change.__repr_syft_nested__()
+                if hasattr(change, "__repr_syft_nested__")
+                else type(change)
+            )
+            str_change = f"{str_change}. "
+            str_changes.append(str_change)
+        str_changes = "\n".join(str_changes)
+        return f"""
+            <style>
+            .syft-request {{color: {SURFACE[options.color_theme]};}}
+            </style>
+            <div class='syft-request'>
+                <h3>Request</h3>
+                <p><strong>Id: </strong>{self.id}</p>
+                <p><strong>Request time: </strong>{self.request_time}</p>
+                {updated_at_line}
+                <p><strong>Changes: </strong> {str_changes}</p>
+                <p><strong>Status: </strong>{self.status}</p>
+            </div>
+            """
+
+    def _coll_repr_(self):
+        if self.status == RequestStatus.APPROVED:
+            badge_color = "badge-green"
+        elif self.status == RequestStatus.PENDING:
+            badge_color = "badge-gray"
+        else:
+            badge_color = "badge-red"
+
+        status_badge = {"value": self.status.name.capitalize(), "type": badge_color}
+        return {
+            "changes": " ".join([x.__repr_syft_nested__() for x in self.changes]),
+            "request time": str(self.request_time),
+            "status": status_badge,
+            "requesting user": {
+                "value": str(self.requesting_user_verify_key),
+                "type": "clipboard",
+            },
+            "reviewed_at": str(self.updated_at),
+        }
+
     @property
-    def status(self) -> RequestStatus:
-        if len(self.history) == 0:
-            return RequestStatus.PENDING
+    def code(self) -> Any:
+        for change in self.changes:
+            if isinstance(change, UserCodeStatusChange):
+                return change.link
 
+        return SyftError(
+            message="This type of request does not have code associated with it."
+        )
+
+    @property
+    def current_change_state(self) -> Dict[UID, bool]:
         change_applied_map = {}
         for change_status in self.history:
             # only store the last change
-            change_applied_map[change_status.id] = change_status.applied
+            change_applied_map[change_status.change_id] = change_status.applied
+
+        return change_applied_map
+
+    @property
+    def icon(self):
+        return REQUEST_ICON
+
+    @property
+    def status(self) -> RequestStatus:
+        if len(self.history) == 0:
+            return RequestStatus.PENDING
 
-        all_changes_applied = all(change_applied_map.values()) and (
-            len(change_applied_map) == len(self.changes)
+        all_changes_applied = all(self.current_change_state.values()) and (
+            len(self.current_change_state) == len(self.changes)
         )
 
         request_status = (
             RequestStatus.APPROVED if all_changes_applied else RequestStatus.REJECTED
         )
 
         return request_status
@@ -182,14 +261,26 @@
     def approve(self):
         api = APIRegistry.api_for(
             self.node_uid,
             self.syft_client_verify_key,
         )
         return api.services.request.apply(self.id)
 
+    def deny(self, reason: str):
+        """Denies the particular request.
+
+        Args:
+            reason (str): Reason for which the request has been denied.
+        """
+        api = APIRegistry.api_for(
+            self.node_uid,
+            self.syft_client_verify_key,
+        )
+        return api.services.request.undo(uid=self.id, reason=reason)
+
     def approve_with_client(self, client):
         return client.api.services.request.apply(self.id)
 
     def apply(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         change_context = ChangeContext.from_service(context)
         change_context.requesting_user_credentials = self.requesting_user_verify_key
         for change in self.changes:
@@ -202,33 +293,57 @@
                 self.save(context=context)
                 return result
 
             # If no error, then change successfully applied.
             change_status.applied = True
             self.history.append(change_status)
 
+        self.updated_at = DateTime.now()
         self.save(context=context)
         return Ok(SyftSuccess(message=f"Request {self.id} changes applied"))
 
+    def undo(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
+        change_context = ChangeContext.from_service(context)
+        change_context.requesting_user_credentials = self.requesting_user_verify_key
+
+        current_change_state = self.current_change_state
+        for change in self.changes:
+            # by default change status is not applied
+            is_change_applied = current_change_state.get(change.id, False)
+            change_status = ChangeStatus(
+                change_id=change.id,
+                applied=is_change_applied,
+            )
+            # undo here may be deny for certain Changes (UserCodeChange)
+            result = change.undo(context=change_context)
+            if result.is_err():
+                # add to history and save history to request
+                self.history.append(change_status)
+                self.save(context=context)
+                return result
+
+            # If no error, then change successfully undoed.
+            change_status.applied = False
+            self.history.append(change_status)
+
+        self.updated_at = DateTime.now()
+        result = self.save(context=context)
+        if isinstance(result, SyftError):
+            return Err(result)
+        # override object with latest changes.
+        self = result
+        return Ok(SyftSuccess(message=f"Request {self.id} changes undoed."))
+
     def save(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         # relative
         from .request_service import RequestService
 
         save_method = context.node.get_service_method(RequestService.save)
         return save_method(context=context, request=self)
 
-    def revert(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
-        change_context = ChangeContext.from_service(context)
-        change_context.requesting_user_credentials = self.requesting_user_verify_key
-        for change in self.changes:
-            result = change.revert(context=change_context)
-            if result.is_err():
-                return result
-        return Ok(SyftSuccess(message=f"Request {self.id} changes reverted"))
-
     def accept_by_depositing_result(self, result: Any, force: bool = False):
         # this code is extremely brittle because its a work around that relies on
         # the type of request being very specifically tied to code which needs approving
         change = self.changes[0]
         if not change.is_type(UserCode):
             raise Exception(
                 f"accept_by_depositing_result can only be run on {UserCode} not "
@@ -243,15 +358,15 @@
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if not api:
             raise Exception(f"Login to {self.node_uid} first.")
 
         is_approved = change.approved
 
         permission_request = self.approve()
-        if not permission_request:
+        if isinstance(permission_request, SyftError):
             return permission_request
 
         code = change.linked_obj.resolve
         state = code.output_policy
 
         # This weird order is due to the fact that state is None before calling approve
         # we could fix it in a future release
@@ -285,29 +400,21 @@
                 action_object, node_uid=self.node_uid
             )
             permission_change = ActionStoreChange(
                 linked_obj=action_object_link,
                 apply_permission_type=ActionPermission.READ,
             )
 
-            submit_request = SubmitRequest(
-                changes=[policy_state_mutation, permission_change],
-                requesting_user_verify_key=self.requesting_user_verify_key,
-            )
+            new_changes = [policy_state_mutation, permission_change]
+            result = api.services.request.add_changes(uid=self.id, changes=new_changes)
+            if isinstance(result, SyftError):
+                return result
+            self = result
 
-            self.approve()
-
-            new_request = api.services.request.submit(submit_request)
-            if not new_request:
-                return new_request
-            new_request_result = api.services.request.apply(new_request.id)
-            if not new_request_result:
-                return new_request_result
-            result = api.services.request.apply(self.id)
-            return result
+            return self.approve()
 
 
 @serializable()
 class RequestInfo(SyftObject):
     # version
     __canonical_name__ = "RequestInfo"
     __version__ = SYFT_OBJECT_VERSION_1
@@ -364,68 +471,93 @@
             "requesting_user_verify_key"
         ] = context.obj.requesting_user_verify_key
     else:
         context.output["requesting_user_verify_key"] = context.credentials
     return context
 
 
+def add_requesting_user_name(context: TransformContext) -> TransformContext:
+    try:
+        user_key = context.output["requesting_user_verify_key"]
+        user_service = context.node.get_service("UserService")
+        user = user_service.get_by_verify_key(user_key)
+        context.output["requesting_user_name"] = user.name
+    except Exception:
+        context.output["requesting_user_name"] = "guest_user"
+    return context
+
+
 @transform(SubmitRequest, Request)
 def submit_request_to_request() -> List[Callable]:
     return [
         generate_id,
         add_node_uid_for_key("node_uid"),
         add_request_time,
         check_requesting_user_verify_key,
+        add_requesting_user_name,
         hash_changes,
     ]
 
 
 @serializable()
 class ObjectMutation(Change):
     __canonical_name__ = "ObjectMutation"
     __version__ = SYFT_OBJECT_VERSION_1
 
     linked_obj: Optional[LinkedObject]
     attr_name: str
     value: Optional[Any]
     match_type: bool
+    previous_value: Optional[Any]
 
-    __attr_repr_cols__ = ["linked_obj", "attr_name"]
+    __repr_attrs__ = ["linked_obj", "attr_name"]
 
-    def mutate(self, obj: Any) -> Any:
+    def mutate(self, obj: Any, value: Optional[Any]) -> Any:
         # check if attribute is a property setter first
         # this seems necessary for pydantic types
         attr = getattr(type(obj), self.attr_name, None)
         if inspect.isdatadescriptor(attr):
-            attr.fset(obj, self.value)
+            self.previous_value = attr.fget(obj)
+            attr.fset(obj, value)
+
         else:
-            setattr(obj, self.attr_name, self.value)
+            self.previous_value = getattr(obj, self.attr_name, None)
+            setattr(obj, self.attr_name, value)
         return obj
 
+    def __repr_syft_nested__(self):
+        return f"Mutate <b>{self.attr_name}</b> to <b>{self.value}</b>"
+
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             obj = self.linked_obj.resolve_with_context(context)
             if obj.is_err():
                 return SyftError(message=obj.err())
             obj = obj.ok()
             if apply:
-                obj = self.mutate(obj)
+                obj = self.mutate(obj, value=self.value)
                 self.linked_obj.update_with_context(context, obj)
             else:
-                raise NotImplementedError
+                # unset the set value
+                obj = self.mutate(obj, value=self.previous_value)
+                self.linked_obj.update_with_context(context, obj)
+
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
-            return Err(SyftError(message=e))
+            return Err(SyftError(message=str(e)))
 
     def apply(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=True)
 
+    def undo(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
+        return self._run(context=context, apply=False)
+
 
 def type_for_field(object_type: type, attr_name: str) -> Optional[type]:
     field_type = None
     try:
         field_type = object_type.__dict__["__annotations__"][attr_name]
     except Exception:  # nosec
         try:
@@ -440,15 +572,15 @@
     __canonical_name__ = "EnumMutation"
     __version__ = SYFT_OBJECT_VERSION_1
 
     enum_type: Type[Enum]
     value: Optional[Enum]
     match_type: bool = True
 
-    __attr_repr_cols__ = ["linked_obj", "attr_name", "value"]
+    __repr_attrs__ = ["linked_obj", "attr_name", "value"]
 
     @property
     def valid(self) -> Union[SyftSuccess, SyftError]:
         if self.match_type and not isinstance(self.value, self.enum_type):
             return SyftError(
                 message=f"{type(self.value)} must be of type: {self.enum_type}"
             )
@@ -488,17 +620,20 @@
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
             return Err(SyftError(message=e))
 
     def apply(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=True)
 
-    def revert(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
+    def undo(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=False)
 
+    def __repr_syft_nested__(self):
+        return f"Mutate <b>{self.enum_type}</b> to <b>{self.value}</b>"
+
     @property
     def link(self) -> Optional[SyftObject]:
         if self.linked_obj:
             return self.linked_obj.resolve
         return None
 
 
@@ -506,21 +641,24 @@
 class UserCodeStatusChange(Change):
     __canonical_name__ = "UserCodeStatusChange"
     __version__ = SYFT_OBJECT_VERSION_1
 
     value: UserCodeStatus
     linked_obj: LinkedObject
     match_type: bool = True
-    __attr_repr_cols__ = [
+    __repr_attrs__ = [
         "link.service_func_name",
         "link.input_policy_type.__canonical_name__",
         "link.output_policy_type.__canonical_name__",
         "link.status.approved",
     ]
 
+    def __repr_syft_nested__(self):
+        return f"Request to change <b>{self.link.service_func_name}</b> to permission <b>RequestStatus.APPROVED</b>"
+
     def _repr_markdown_(self) -> str:
         link = self.link
         input_policy_type = (
             link.input_policy_type.__canonical_name__
             if link.input_policy_type is not None
             else None
         )
@@ -545,20 +683,27 @@
     def valid(self) -> Union[SyftSuccess, SyftError]:
         if self.match_type and not isinstance(self.value, UserCodeStatus):
             return SyftError(
                 message=f"{type(self.value)} must be of type: {UserCodeStatus}"
             )
         return SyftSuccess(message=f"{type(self)} valid")
 
-    def mutate(self, obj: UserCode, context: ChangeContext) -> Any:
-        res = obj.status.mutate(
-            value=self.value,
-            node_name=context.node.name,
-            verify_key=context.node.signing_key.verify_key,
-        )
+    def mutate(self, obj: UserCode, context: ChangeContext, undo: bool) -> Any:
+        if not undo:
+            res = obj.status.mutate(
+                value=self.value,
+                node_name=context.node.name,
+                verify_key=context.node.signing_key.verify_key,
+            )
+        else:
+            res = obj.status.mutate(
+                value=UserCodeStatus.DENIED,
+                node_name=context.node.name,
+                verify_key=context.node.signing_key.verify_key,
+            )
         if res.is_ok():
             obj.status = res.ok()
             return Ok(obj)
         return res
 
     def _run(
         self, context: ChangeContext, apply: bool
@@ -568,15 +713,15 @@
             if not valid:
                 return Err(valid)
             obj = self.linked_obj.resolve_with_context(context)
             if obj.is_err():
                 return SyftError(message=obj.err())
             obj = obj.ok()
             if apply:
-                res = self.mutate(obj, context)
+                res = self.mutate(obj, context, undo=False)
 
                 if res.is_err():
                     return res
                 res = res.ok()
                 if OBLV:
                     # relative
                     from ...external.oblv.oblv_service import check_enclave_transfer
@@ -587,24 +732,31 @@
                 else:
                     enclave_res = Ok()
 
                 if enclave_res.is_err():
                     return enclave_res
                 self.linked_obj.update_with_context(context, res)
             else:
-                raise NotImplementedError
+                res = self.mutate(obj, context, undo=True)
+                if res.is_err():
+                    return res
+
+                res = res.ok()
+
+                # TODO: Handle Enclave approval.
+                self.linked_obj.update_with_context(context, res)
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
             return Err(SyftError(message=str(e)))
 
     def apply(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=True)
 
-    def revert(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
+    def undo(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=False)
 
     @property
     def link(self) -> Optional[SyftObject]:
         if self.linked_obj:
             return self.linked_obj.resolve
         return None
```

### Comparing `syft-0.8.1b9/src/syft/service/request/request_service.py` & `syft-0.8.2b1/src/syft/service/request/request_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user import UserView
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..user.user_service import UserService
+from .request import Change
 from .request import Request
 from .request import RequestInfo
 from .request import RequestInfoFilter
 from .request import SubmitRequest
 from .request_stash import RequestStash
 
 
@@ -70,16 +71,18 @@
                 link = LinkedObject.with_context(request, context=context)
                 admin_verify_key = context.node.get_service_method(
                     UserService.admin_verify_key
                 )
 
                 root_verify_key = admin_verify_key()
                 if send_message:
+                    subject_msg = f"Result to request {str(request.id)[:4]}...{str(request.id)[-3:]}\
+                        has been successfully deposited."
                     message = CreateMessage(
-                        subject="Approval Request" if not reason else reason,
+                        subject=subject_msg if not reason else reason,
                         from_user_verify_key=context.credentials,
                         to_user_verify_key=root_verify_key,
                         linked_obj=link,
                     )
                     method = context.node.get_service_method(MessageService.send)
                     result = method(context=context, message=message)
                     if isinstance(result, Message):
@@ -132,14 +135,29 @@
                 # Return the proper slice using chunk_index
                 requests = requests[page_index]
 
             return requests
 
         return SyftError(message=result.err())
 
+    @service_method(path="request.add_changes", name="add_changes")
+    def add_changes(
+        self, context: AuthedServiceContext, uid: UID, changes: List[Change]
+    ) -> Union[Request, SyftError]:
+        result = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
+
+        if result.is_err():
+            return SyftError(
+                message=f"Failed to retrieve request with uid: {uid}. Error: {result.err()}"
+            )
+
+        request = result.ok()
+        request.changes.extend(changes)
+        return self.save(context=context, request=request)
+
     @service_method(path="request.filter_all_info", name="filter_all_info")
     def filter_all_info(
         self,
         context: AuthedServiceContext,
         request_filter: RequestInfoFilter,
         page_index: Optional[int] = 0,
         page_size: Optional[int] = 0,
@@ -167,32 +185,57 @@
         request = self.stash.get_by_uid(context.credentials, uid)
         if request.is_ok():
             request = request.ok()
             result = request.apply(context=context)
             return result.value
         return request.value
 
-    @service_method(path="request.revert", name="revert")
-    def revert(
-        self, context: AuthedServiceContext, uid: UID
+    @service_method(path="request.undo", name="undo")
+    def undo(
+        self, context: AuthedServiceContext, uid: UID, reason: str
     ) -> Union[SyftSuccess, SyftError]:
-        request = self.stash.get_by_uid(uid)
-        if request.is_ok():
-            result = request.ok().revert(context=context)
-            return result.value
-        return request.value
+        result = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
+        if result.is_err():
+            return SyftError(
+                message=f"Failed to update request: {uid} with error: {result.err()}"
+            )
+
+        request = result.ok()
+        if request is None:
+            return SyftError(message=f"Request with uid: {uid} does not exists.")
+
+        result = request.undo(context=context)
+
+        if result.is_err():
+            return SyftError(
+                f"Failed to undo Request: <{uid}> with error: {result.err()}"
+            )
+
+        link = LinkedObject.with_context(request, context=context)
+        message_subject = (
+            f"Your request for uid: {uid} has been denied. "
+            f"Reason specified by Data Owner: {reason}."
+        )
+
+        notification = CreateMessage(
+            subject=message_subject,
+            to_user_verify_key=request.requesting_user_verify_key,
+            linked_obj=link,
+        )
+        send_notification = context.node.get_service_method(MessageService.send)
+
+        result = send_notification(context=context, message=notification)
+        return SyftSuccess(message=f"Request {uid} successfully denied !")
 
     def save(
         self, context: AuthedServiceContext, request: Request
-    ) -> Union[SyftSuccess, SyftError]:
+    ) -> Union[Request, SyftError]:
         result = self.stash.update(context.credentials, request)
         if result.is_ok():
-            return SyftSuccess(
-                message=f"Request: {request.id} updated successfully !!!"
-            )
+            return result.ok()
         return SyftError(
             message=f"Failed to update Request: <{request.id}>. Error: {result.err()}"
         )
 
 
 TYPE_TO_SERVICE[Request] = RequestService
 SERVICE_TO_TYPES[RequestService].update({Request})
```

### Comparing `syft-0.8.1b9/src/syft/service/request/request_stash.py` & `syft-0.8.2b1/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/response.py` & `syft-0.8.2b1/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/service.py` & `syft-0.8.2b1/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/settings/settings.py` & `syft-0.8.2b1/src/syft/service/settings/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # stdlib
-from typing import Optional
 
 # relative
 from ...serde.serializable import serializable
+from ...types.syft_object import PartialSyftObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.uid import UID
 
 
 @serializable()
-class NodeSettingsUpdate(SyftObject):
+class NodeSettingsUpdate(PartialSyftObject):
     __canonical_name__ = "NodeSettingsUpdate"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    id: Optional[UID]
-    name: Optional[str]
-    organization: Optional[str]
-    description: Optional[str]
-    on_board: Optional[bool]
+    id: UID
+    name: str
+    organization: str
+    description: str
+    on_board: bool
+    signup_enabled: bool
 
 
 @serializable()
 class NodeSettings(SyftObject):
     __canonical_name__ = "NodeSettings"
     __version__ = SYFT_OBJECT_VERSION_1
+    __repr_attrs__ = ["name", "organization", "deployed_on", "signup_enabled"]
 
     name: str = "Node"
     deployed_on: str
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "Text"
+    signup_enabled: bool
```

### Comparing `syft-0.8.1b9/src/syft/service/settings/settings_service.py` & `syft-0.8.2b1/src/syft/service/settings/settings_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # stdlib
 
+# stdlib
+from typing import Union
+
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
+from ...util.experimental_flags import flags
 from ..context import AuthedServiceContext
 from ..context import UnauthedServiceContext
 from ..response import SyftError
+from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import service_method
 from .settings import NodeSettings
 from .settings import NodeSettingsUpdate
 from .settings_stash import SettingsStash
 
 
@@ -58,18 +63,35 @@
         self, context: AuthedServiceContext, settings: NodeSettingsUpdate
     ) -> Result[Ok, Err]:
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             current_settings = result.ok()
             if len(current_settings) > 0:
                 new_settings = current_settings[0].copy(
-                    update=settings.dict(exclude_unset=True)
+                    update=settings.to_dict(exclude_empty=True)
                 )
                 update_result = self.stash.update(context.credentials, new_settings)
                 if update_result.is_ok():
                     return result
                 else:
                     return SyftError(message=update_result.err())
             else:
                 return SyftError(message="No settings found")
         else:
             return SyftError(message=result.err())
+
+    @service_method(path="settings.allow_guest_signup", name="allow_guest_signup")
+    def allow_guest_signup(
+        self, context: AuthedServiceContext, enable: bool
+    ) -> Union[SyftSuccess, SyftError]:
+        """Enable/Disable Registration for Data Scientist or Guest Users."""
+        flags.CAN_REGISTER = enable
+        method = context.node.get_service_method(SettingsService.update)
+        settings = NodeSettingsUpdate(signup_enabled=enable)
+
+        result = method(context=context, settings=settings)
+
+        if result.is_err():
+            return SyftError(message=f"Failed to update settings: {result.err()}")
+
+        message = "enabled" if enable else "disabled"
+        return SyftSuccess(message=f"Registration feature successfully {message}")
```

### Comparing `syft-0.8.1b9/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b1/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/user/user.py` & `syft-0.8.2b1/src/syft/service/user/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # stdlib
+from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 # third party
 from bcrypt import checkpw
 from bcrypt import gensalt
@@ -52,24 +54,25 @@
     institution: Optional[str]
     website: Optional[str] = None
     created_at: Optional[str] = None
 
     # serde / storage rules
     __attr_searchable__ = ["name", "email", "verify_key", "role"]
     __attr_unique__ = ["email", "signing_key", "verify_key"]
-    __attr_repr_cols__ = ["name", "email"]
+    __repr_attrs__ = ["name", "email"]
 
 
 def default_role(role: ServiceRole) -> Callable:
     return make_set_default(key="role", value=role)
 
 
 def hash_password(context: TransformContext) -> TransformContext:
     if context.output["password"] is not None and (
-        context.output["password"] == context.output["password_verify"]
+        (context.output["password_verify"] is None)
+        or context.output["password"] == context.output["password_verify"]
     ):
         salt, hashed = salt_and_hash_password(context.output["password"], 12)
         context.output["hashed_password"] = hashed
         context.output["salt"] = salt
     return context
 
 
@@ -120,20 +123,21 @@
     __canonical_name__ = "UserCreate"
     __version__ = SYFT_OBJECT_VERSION_1
 
     email: EmailStr
     name: str
     role: Optional[ServiceRole] = None  # make sure role cant be set without uid
     password: str
-    password_verify: str
+    password_verify: Optional[str] = None
     verify_key: Optional[SyftVerifyKey]
     institution: Optional[str]
     website: Optional[str]
+    created_by: Optional[SyftSigningKey]
 
-    __attr_repr_cols__ = ["name", "email"]
+    __repr_attrs__ = ["name", "email"]
 
 
 @serializable()
 class UserSearch(PartialSyftObject):
     __canonical_name__ = "UserSearch"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -150,15 +154,24 @@
 
     email: EmailStr
     name: str
     role: ServiceRole  # make sure role cant be set without uid
     institution: Optional[str]
     website: Optional[str]
 
-    __attr_repr_cols__ = ["name", "email"]
+    __repr_attrs__ = ["name", "email", "institute", "website", "role"]
+
+    def _coll_repr_(self) -> Dict[str, Any]:
+        return {
+            "Name": self.name,
+            "Email": self.email,
+            "Institute": self.institution,
+            "Website": self.website,
+            "Role": self.role.name.capitalize(),
+        }
 
 
 @transform(UserUpdate, User)
 def user_update_to_user() -> List[Callable]:
     return [
         validate_email,
         hash_password,
@@ -169,17 +182,17 @@
 @transform(UserCreate, User)
 def user_create_to_user() -> List[Callable]:
     return [
         generate_id,
         validate_email,
         hash_password,
         generate_key,
+        drop(["password", "password_verify", "created_by"]),
         # TODO: Fix this by passing it from client & verifying it at server
         default_role(ServiceRole.DATA_SCIENTIST),
-        drop(["password", "password_verify"]),
     ]
 
 
 @transform(User, UserView)
 def user_to_view_user() -> List[Callable]:
     return [keep(["id", "email", "name", "role", "institution", "website"])]
```

### Comparing `syft-0.8.1b9/src/syft/service/user/user_roles.py` & `syft-0.8.2b1/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/user/user_service.py` & `syft-0.8.2b1/src/syft/service/user/user_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # stdlib
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 # relative
+from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...node.credentials import UserLoginCredentials
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.syft_metaclass import Empty
 from ...types.uid import UID
 from ...util.telemetry import instrument
@@ -113,20 +114,26 @@
 
             return results
 
         # 🟡 TODO: No user exists will happen when result.ok() is empty list
         return SyftError(message="No users exists")
 
     def get_role_for_credentials(
-        self, credentials: SyftVerifyKey
+        self, credentials: Union[SyftVerifyKey, SyftSigningKey]
     ) -> Union[Optional[ServiceRole], SyftError]:
         # they could be different
-        result = self.stash.get_by_verify_key(
-            credentials=credentials, verify_key=credentials
-        )
+
+        if isinstance(credentials, SyftVerifyKey):
+            result = self.stash.get_by_verify_key(
+                credentials=credentials, verify_key=credentials
+            )
+        else:
+            result = self.stash.get_by_signing_key(
+                credentials=credentials, signing_key=credentials
+            )
         if result.is_ok():
             # this seems weird that we get back None as Ok(None)
             user = result.ok()
             if user:
                 return user.role
         return ServiceRole.GUEST
 
@@ -326,14 +333,29 @@
             return SyftError(message=str(e))
 
     def register(
         self, context: NodeServiceContext, new_user: UserCreate
     ) -> Union[Tuple[SyftSuccess, UserPrivateKey], SyftError]:
         """Register new user"""
 
+        request_user_role = (
+            ServiceRole.GUEST
+            if new_user.created_by is None
+            else self.get_role_for_credentials(new_user.created_by)
+        )
+        can_user_register = context.node.metadata.signup_enabled or (
+            request_user_role in DATA_OWNER_ROLE_LEVEL
+        )
+
+        if not can_user_register:
+            return SyftError(
+                message=f"You don't have permission to create an account "
+                f"on the domain: {context.node.name}. Please contact the Domain Owner."
+            )
+
         user = new_user.to(User)
         result = self.stash.get_by_email(credentials=user.verify_key, email=user.email)
         if result.is_err():
             return SyftError(message=str(result.err()))
         user_exists = result.ok() is not None
         if user_exists:
             return SyftError(message=f"User already exists with email: {user.email}")
@@ -347,15 +369,19 @@
                 ),
             ],
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         user = result.ok()
-        msg = SyftSuccess(message="User successfully registered!")
+
+        success_message = f"User '{user.name}' successfully registered!"
+        if request_user_role in DATA_OWNER_ROLE_LEVEL:
+            success_message += " To see users, run `[your_client].users`"
+        msg = SyftSuccess(message=success_message)
         return tuple([msg, user.to(UserPrivateKey)])
 
     def user_verify_key(self, email: str) -> Union[SyftVerifyKey, SyftError]:
         # we are bypassing permissions here, so dont use to return a result directly to the user
         credentials = self.admin_verify_key()
         result = self.stash.get_by_email(credentials=credentials, email=email)
         if result.is_ok():
```

### Comparing `syft-0.8.1b9/src/syft/service/user/user_stash.py` & `syft-0.8.2b1/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b1/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b1/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/service/vpn/vpn.py` & `syft-0.8.2b1/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/dict_document_store.py` & `syft-0.8.2b1/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/document_store.py` & `syft-0.8.2b1/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/kv_document_store.py` & `syft-0.8.2b1/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/linked_obj.py` & `syft-0.8.2b1/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/locks.py` & `syft-0.8.2b1/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/mongo_client.py` & `syft-0.8.2b1/src/syft/store/mongo_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,18 +97,18 @@
 
     """
 
     # Connection
     hostname: Optional[str] = "127.0.0.1"
     port: Optional[int] = None
     directConnection: bool = False
-    maxPoolSize: int = 100
+    maxPoolSize: int = 200
     minPoolSize: int = 0
     maxIdleTimeMS: Optional[int] = None
-    maxConnecting: int = 2
+    maxConnecting: int = 3
     timeoutMS: int = 0
     socketTimeoutMS: int = 0
     connectTimeoutMS: int = 20000
     serverSelectionTimeoutMS: int = 30000
     waitQueueTimeoutMS: Optional[int] = None
     heartbeatFrequencyMS: int = 10000
     appname: str = "pysyft"
```

### Comparing `syft-0.8.1b9/src/syft/store/mongo_codecs.py` & `syft-0.8.2b1/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/store/mongo_document_store.py` & `syft-0.8.2b1/src/syft/store/mongo_document_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ..node.credentials import SyftVerifyKey
+from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
+from ..serde.serialize import _serialize
 from ..service.action.action_permissions import ActionObjectPermission
 from ..service.action.action_permissions import ActionObjectREAD
 from ..service.action.action_permissions import ActionObjectWRITE
 from ..service.response import SyftSuccess
 from ..types.syft_object import StorableObjectType
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
-from ..types.syft_object import SyftObjectRegistry
 from ..types.transforms import TransformContext
 from ..types.transforms import transform
 from ..types.transforms import transform_method
 from .document_store import DocumentStore
 from .document_store import PartitionKey
 from .document_store import QueryKey
 from .document_store import QueryKeys
@@ -82,43 +83,30 @@
         else:
             output[k] = value
 
     if "id" in context.output:
         output["_id"] = context.output["id"]
     output["__canonical_name__"] = context.obj.__canonical_name__
     output["__version__"] = context.obj.__version__
-    mongo_dict = MongoDict.from_dict(context.obj.to_dict())
-    output["__obj__"] = mongo_dict
+    output["__blob__"] = _serialize(context.obj, to_bytes=True)
     output["__arepr__"] = _repr_debug_(context.obj)  # a comes first in alphabet
     context.output = output
     return context
 
 
 @transform(SyftObject, MongoBsonObject)
 def syft_obj_to_mongo():
     return [to_mongo]
 
 
 @transform_method(MongoBsonObject, SyftObject)
 def from_mongo(
     storage_obj: Dict, context: Optional[TransformContext] = None
 ) -> SyftObject:
-    constructor = SyftObjectRegistry.versioned_class(
-        name=storage_obj["__canonical_name__"], version=storage_obj["__version__"]
-    )
-    if constructor is None:
-        raise ValueError(
-            "Versioned class should not be None for initialization of SyftObject."
-        )
-    mongo_dict = storage_obj["__obj__"]
-    output = mongo_dict.dict
-    for attr, funcs in constructor.__serde_overrides__.items():
-        if attr in output:
-            output[attr] = funcs[1](output[attr])
-    return constructor(**output)
+    return _deserialize(storage_obj["__blob__"], from_bytes=True)
 
 
 @serializable(attrs=["storage_type"])
 class MongoStorePartition(StorePartition):
     """Mongo StorePartition
 
     Parameters:
```

### Comparing `syft-0.8.1b9/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b1/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/types/datetime.py` & `syft-0.8.2b1/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/types/grid_url.py` & `syft-0.8.2b1/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/types/syft_metaclass.py` & `syft-0.8.2b1/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/types/syft_object.py` & `syft-0.8.2b1/src/syft/types/syft_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 from typing import Sequence
 from typing import Tuple
 from typing import Type
 from typing import Union
 import warnings
 
 # third party
-import itables
+import pandas as pd
 import pydantic
 from pydantic import BaseModel
 from pydantic import EmailStr
 from pydantic.fields import Undefined
 from result import OkErr
 from typeguard import check_type
 
 # relative
 from ..node.credentials import SyftVerifyKey
-from ..serde.deserialize import _deserialize as deserialize
 from ..serde.recursive_primitives import recursive_serde_register_type
 from ..serde.serialize import _serialize as serialize
 from ..util.autoreload import autoreload_enabled
 from ..util.markdown import as_markdown_python_code
+from ..util.notebook_ui.notebook_addons import create_table_template
 from ..util.util import aggressive_set_attr
 from ..util.util import full_name_with_qualname
 from ..util.util import get_qualname_for
 from .syft_metaclass import Empty
 from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
 
@@ -60,28 +60,14 @@
 # These attributes are dynamically added based on node/client
 # that is interaction with the SyftObject
 DYNAMIC_SYFT_ATTRIBUTES = [
     "syft_node_location",
     "syft_client_verify_key",
 ]
 
-SURFACE_DARK_BRIGHT = "#464158"
-SURFACE_SURFACE = "#2E2B3B"
-DK_ON_SURFACE_HIGHEST = "#534F64"
-
-# This can be customize however we want
-itables_css = f"""
-.itables table {{
-    margin: 0 auto;
-    float: left;
-    color: {DK_ON_SURFACE_HIGHEST};
-}}
-.itables table th {{color: {SURFACE_SURFACE};}}
-"""
-
 
 class SyftHashableObject:
     __hash_exclude_attrs__ = []
 
     def __hash__(self) -> int:
         return int.from_bytes(self.__sha256__(), byteorder="big")
 
@@ -216,42 +202,19 @@
     __attr_unique__: ClassVar[List[str]] = []
     # the unique keys for the particular Collection the objects will be stored in
     __serde_overrides__: Dict[
         str, Sequence[Callable]
     ] = {}  # List of attributes names which require a serde override.
     __owner__: str
 
-    __attr_repr_cols__: ClassVar[List[str]] = []  # show these in html repr collections
+    __repr_attrs__: ClassVar[List[str]] = []  # show these in html repr collections
     __attr_custom_repr__: ClassVar[
         List[str]
     ] = None  # show these in html repr of an object
 
-    def to_mongo(self) -> Dict[str, Any]:
-        warnings.warn(
-            "`SyftObject.to_mongo` is deprecated and will be removed in a future version",
-            PendingDeprecationWarning,
-        )
-
-        d = {}
-        for k in self.__attr_searchable__:
-            # 🟡 TODO 24: pass in storage abstraction and detect unsupported types
-            # if unsupported, convert to string
-            value = getattr(self, k, "")
-            if isinstance(value, SyftVerifyKey):
-                value = str(value)
-            d[k] = value
-        blob = serialize(dict(self), to_bytes=True)
-        d["_id"] = self.id.value  # type: ignore
-        d["__canonical_name__"] = self.__canonical_name__
-        d["__version__"] = self.__version__
-        d["__blob__"] = blob
-        d["__repr__"] = self.__repr__()
-
-        return d
-
     def __syft_get_funcs__(self) -> List[Tuple[str, Signature]]:
         funcs = print_type_cache[type(self)]
         if len(funcs) > 0:
             return funcs
 
         for attr in dir(type(self)):
             obj = getattr(type(self), attr, None)
@@ -292,34 +255,47 @@
         return _repr_str
 
     def _repr_markdown_(self, wrap_as_python=True, indent=0) -> str:
         s_indent = " " * indent * 2
         class_name = get_qualname_for(type(self))
         if self.__attr_custom_repr__ is not None:
             fields = self.__attr_custom_repr__
-        elif self.__attr_repr_cols__ is not None:
-            fields = self.__attr_repr_cols__
+        elif self.__repr_attrs__ is not None:
+            fields = self.__repr_attrs__
         else:
             fields = list(getattr(self, "__fields__", {}).keys())
 
         if "id" not in fields:
             fields = ["id"] + fields
 
         dynam_attrs = set(DYNAMIC_SYFT_ATTRIBUTES)
         fields = [x for x in fields if x not in dynam_attrs]
         _repr_str = f"{s_indent}class {class_name}:\n"
         for attr in fields:
             value = self
-            if getattr(value, attr, None) is None:
-                value = getattr(value, attr, "<Missing>")
-            else:
-                for _attr in attr.split("."):  # if compound string
+            # if it's a compound string
+            if "." in attr:
+                # break it into it's bits & fetch the attr
+                for _attr in attr.split("."):
                     value = getattr(value, _attr, "<Missing>")
+            else:
+                value = getattr(value, attr, "<Missing>")
+
             value_type = full_name_with_qualname(type(attr))
             value_type = value_type.replace("builtins.", "")
+            # If the object has a special representation when nested we will use that instead
+            if hasattr(value, "__repr_syft_nested__"):
+                value = value.__repr_syft_nested__()
+            if isinstance(value, list):
+                value = [
+                    elem.__repr_syft_nested__()
+                    if hasattr(elem, "__repr_syft_nested__")
+                    else elem
+                    for elem in value
+                ]
             value = f'"{value}"' if isinstance(value, str) else value
             _repr_str += f"{s_indent}  {attr}: {value_type} = {value}\n"
 
         # _repr_str += "\n"
         # fqn = full_name_with_qualname(type(self))
         # _repr_str += f'fqn = "{fqn}"\n'
         # _repr_str += f"mro = {[t.__name__ for t in type(self).mro()]}"
@@ -330,34 +306,14 @@
         # _repr_str += f"]"
         # return _repr_str
         if wrap_as_python:
             return as_markdown_python_code(_repr_str)
         else:
             return _repr_str
 
-    @staticmethod
-    def from_mongo(bson: Any) -> "SyftObject":
-        warnings.warn(
-            "`SyftObject.from_mongo` is deprecated and will be removed in a future version",
-            PendingDeprecationWarning,
-        )
-
-        constructor = SyftObjectRegistry.versioned_class(
-            name=bson["__canonical_name__"], version=bson["__version__"]
-        )
-        if constructor is None:
-            raise ValueError(
-                "Versioned class should not be None for initialization of SyftObject."
-            )
-        de = deserialize(bson["__blob__"], from_bytes=True)
-        for attr, funcs in constructor.__serde_overrides__.items():
-            if attr in de:
-                de[attr] = funcs[1](de[attr])
-        return constructor(**de)
-
     # allows splatting with **
     def keys(self) -> KeysView[str]:
         return self.__dict__.keys()
 
     # allows splatting with **
     def __getitem__(self, key: str) -> Any:
         return self.__dict__.__getitem__(key)
@@ -536,92 +492,118 @@
             elif hasattr(item, "mro") and type(item) != type:
                 mro = item.mro()
             else:
                 mro = str(self)
 
             if "syft" in str(mro).lower():
                 has_syft = True
-                extra_fields = getattr(item, "__attr_repr_cols__", [])
+                extra_fields = getattr(item, "__repr_attrs__", [])
                 break
         if has_syft:
             # third party
-            import pandas as pd
+            first_value = values[0]
+            if is_homogenous:
+                cls_name = first_value.__class__.__name__
+            else:
+                cls_name = ""
 
             cols = defaultdict(list)
-            # max_lines = 5
-            line = 0
             for item in iter(self):
-                line += 1
-                # if line > max_lines:
-                #     break
+                # unpack dict
                 if isinstance(self, dict):
                     cols["key"].append(item)
                     item = self.__getitem__(item)
 
                 # get id
                 id_ = getattr(item, "id", None)
-                if id is not None:
-                    id_ = f"{str(id_)[:4]}...{str(id_)[-3:]}"
+                if id_ is not None:
+                    cols["id"].append({"value": str(id_), "type": "clipboard"})
 
                 if type(item) == type:
                     t = full_name_with_qualname(item)
                 else:
                     try:
                         t = item.__class__.__name__
                     except Exception:
                         t = item.__repr__()
-                cols["id"].append(id_)
+
                 if not is_homogenous:
                     cols["type"].append(t)
 
-                for field in extra_fields:
-                    value = item
-                    try:
-                        attrs = field.split(".")
-                        for attr in attrs:
-                            # find indexing like abc[1]
-                            res = re.search("\[[+-]?\d+\]", attr)
-                            has_index = False
-                            if res:
-                                has_index = True
-                                index_str = res.group()
-                                index = int(index_str.replace("[", "").replace("]", ""))
-                                attr = attr.replace(index_str, "")
-
-                            value = getattr(value, attr, None)
-                            if isinstance(value, list) and has_index:
-                                value = value[index]
-                    except Exception as e:
-                        print(e)
-                        value = None
-                    cols[field].append(value)
+                # if has _coll_repr_
+                if hasattr(item, "_coll_repr_"):
+                    ret_val = item._coll_repr_()
+                    if "id" in ret_val:
+                        del ret_val["id"]
+                    for key in ret_val.keys():
+                        cols[key].append(ret_val[key])
+                else:
+                    for field in extra_fields:
+                        value = item
+                        try:
+                            attrs = field.split(".")
+                            for i, attr in enumerate(attrs):
+                                # find indexing like abc[1]
+                                res = re.search("\[[+-]?\d+\]", attr)
+                                has_index = False
+                                if res:
+                                    has_index = True
+                                    index_str = res.group()
+                                    index = int(
+                                        index_str.replace("[", "").replace("]", "")
+                                    )
+                                    attr = attr.replace(index_str, "")
+
+                                value = getattr(value, attr, None)
+                                if isinstance(value, list) and has_index:
+                                    value = value[index]
+                                # If the object has a special representation when nested we will use that instead
+                                if (
+                                    hasattr(value, "__repr_syft_nested__")
+                                    and i == len(attrs) - 1
+                                ):
+                                    value = value.__repr_syft_nested__()
+                                if (
+                                    isinstance(value, list)
+                                    and i == len(attrs) - 1
+                                    and len(value) > 0
+                                    and hasattr(value[0], "__repr_syft_nested__")
+                                ):
+                                    value = [
+                                        x.__repr_syft_nested__()
+                                        if hasattr(x, "__repr_syft_nested__")
+                                        else x
+                                        for x in value
+                                    ]
+                            if value is None:
+                                value = "n/a"
+
+                        except Exception as e:
+                            print(e)
+                            value = None
+                        cols[field].append(str(value))
 
             df = pd.DataFrame(cols)
 
-            if is_homogenous:
-                cls_name = values[0].__class__.__name__
-            else:
-                cls_name = ""
-
-            html_header = f"""
-                <style>
-                .collection-header {{color: {SURFACE_DARK_BRIGHT};}}
-                </style>
-                <div class='collection-header'>
-                    <h3>{cls_name} {self.__class__.__name__.capitalize()}</h3>
-                </div>
-                <br>
-                """
+            if "created_at" in df.columns:
+                df.sort_values(by="created_at", ascending=False, inplace=True)
 
-            html_datatable = itables.to_html_datatable(df=df, css=itables_css)
+            # if custom_repr:
+            table_icon = None
+            if hasattr(values[0], "icon"):
+                table_icon = values[0].icon
+            # this is a list of dicts
+            return create_table_template(
+                df.to_dict("records"),
+                f"{cls_name} {self.__class__.__name__.capitalize()}",
+                table_icon=table_icon,
+            )
 
-            return html_header + html_datatable
-            # return collection_type + df_styled._repr_html_()
     except Exception as e:
-        print(e)
+        print(f"error representing {type(self)} of objects. {e}")
         pass
 
     # stdlib
     import html
 
     return html.escape(self.__repr__())
```

### Comparing `syft-0.8.1b9/src/syft/types/transforms.py` & `syft-0.8.2b1/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/types/twin_object.py` & `syft-0.8.2b1/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/types/uid.py` & `syft-0.8.2b1/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/util/autoreload.py` & `syft-0.8.2b1/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/util/decorators.py` & `syft-0.8.2b1/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/util/experimental_flags.py` & `syft-0.8.2b1/src/syft/util/experimental_flags.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,20 @@
     NONE = 0
 
 
 class ExperimentalFlags:
     def __init__(self) -> None:
         self._APACHE_ARROW_TENSOR_SERDE = True
         self._APACHE_ARROW_COMPRESSION = ApacheArrowCompression.ZSTD
+        self._CAN_REGISTER = str_to_bool(
+            os.getenv(
+                "ENABLE_SIGNUP",
+                "False",
+            )
+        )
 
     @property
     def APACHE_ARROW_TENSOR_SERDE(self) -> bool:
         return self._APACHE_ARROW_TENSOR_SERDE
 
     @APACHE_ARROW_TENSOR_SERDE.getter
     def APACHE_ARROW_TENSOR_SERDE(self) -> bool:
@@ -41,9 +47,17 @@
     def APACHE_ARROW_COMPRESSION(self, value: ApacheArrowCompression) -> None:
         self._APACHE_ARROW_COMPRESSION = value
 
     @property
     def USE_NEW_SERVICE(self) -> bool:
         return str_to_bool(os.getenv("USE_NEW_SERVICE", "False"))
 
+    @property
+    def CAN_REGISTER(self) -> bool:
+        return self._CAN_REGISTER
+
+    @CAN_REGISTER.setter
+    def CAN_REGISTER(self, value: bool) -> None:
+        self._CAN_REGISTER = value
+
 
 flags = ExperimentalFlags()
```

### Comparing `syft-0.8.1b9/src/syft/util/logger.py` & `syft-0.8.2b1/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/util/schema.py` & `syft-0.8.2b1/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/util/telemetry.py` & `syft-0.8.2b1/src/syft/util/telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,62 +22,67 @@
 
 
 T = TypeVar("T", bound=Union[Callable, type])
 P = ParamSpec("P")
 
 
 def setup_tracer() -> Callable[Concatenate[T, P], T]:
-    if not TRACE_MODE:
-
-        def noop(func: T) -> T:
-            return func
+    def noop(func: T) -> T:
+        return func
 
+    if not TRACE_MODE:
         return noop
 
-    print("OpenTelemetry Tracing enabled")
-    service_name = os.environ.get("SERVICE_NAME", "client")
-    jaeger_host = os.environ.get("JAEGER_HOST", "localhost")
-    jaeger_port = int(os.environ.get("JAEGER_PORT", "14268"))
-
-    # third party
-    from opentelemetry import trace
-    from opentelemetry.exporter.jaeger.thrift import JaegerExporter
-    from opentelemetry.sdk.resources import Resource
-    from opentelemetry.sdk.resources import SERVICE_NAME
-    from opentelemetry.sdk.trace import TracerProvider
-    from opentelemetry.sdk.trace.export import BatchSpanProcessor
-
-    trace.set_tracer_provider(
-        TracerProvider(resource=Resource.create({SERVICE_NAME: service_name}))
-    )
-    jaeger_exporter = JaegerExporter(
-        # agent_host_name=jaeger_host,
-        # agent_port=jaeger_port,
-        collector_endpoint=f"http://{jaeger_host}:{jaeger_port}/api/traces?format=jaeger.thrift",
-        # udp_split_oversized_batches=True,
-    )
-
-    trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(jaeger_exporter))
-
-    # from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-    # console_exporter = ConsoleSpanExporter()
-    # span_processor = BatchSpanProcessor(console_exporter)
-    # trace.get_tracer_provider().add_span_processor(span_processor)
-
-    # third party
-    import opentelemetry.instrumentation.requests
-
-    opentelemetry.instrumentation.requests.RequestsInstrumentor().instrument()
-
-    # relative
-    # from opentelemetry.instrumentation.digma.trace_decorator import (
-    #     instrument as _instrument,
-    # )
-    #
-    # until this is merged:
-    # https://github.com/digma-ai/opentelemetry-instrumentation-digma/pull/41
-    from .trace_decorator import instrument as _instrument
-
-    return _instrument
+    try:
+        print("OpenTelemetry Tracing enabled")
+        service_name = os.environ.get("SERVICE_NAME", "client")
+        jaeger_host = os.environ.get("JAEGER_HOST", "localhost")
+        jaeger_port = int(os.environ.get("JAEGER_PORT", "14268"))
+
+        # third party
+        from opentelemetry import trace
+        from opentelemetry.exporter.jaeger.thrift import JaegerExporter
+        from opentelemetry.sdk.resources import Resource
+        from opentelemetry.sdk.resources import SERVICE_NAME
+        from opentelemetry.sdk.trace import TracerProvider
+        from opentelemetry.sdk.trace.export import BatchSpanProcessor
+
+        trace.set_tracer_provider(
+            TracerProvider(resource=Resource.create({SERVICE_NAME: service_name}))
+        )
+        jaeger_exporter = JaegerExporter(
+            # agent_host_name=jaeger_host,
+            # agent_port=jaeger_port,
+            collector_endpoint=f"http://{jaeger_host}:{jaeger_port}/api/traces?format=jaeger.thrift",
+            # udp_split_oversized_batches=True,
+        )
+
+        trace.get_tracer_provider().add_span_processor(
+            BatchSpanProcessor(jaeger_exporter)
+        )
+
+        # from opentelemetry.sdk.trace.export import ConsoleSpanExporter
+        # console_exporter = ConsoleSpanExporter()
+        # span_processor = BatchSpanProcessor(console_exporter)
+        # trace.get_tracer_provider().add_span_processor(span_processor)
+
+        # third party
+        import opentelemetry.instrumentation.requests
+
+        opentelemetry.instrumentation.requests.RequestsInstrumentor().instrument()
+
+        # relative
+        # from opentelemetry.instrumentation.digma.trace_decorator import (
+        #     instrument as _instrument,
+        # )
+        #
+        # until this is merged:
+        # https://github.com/digma-ai/opentelemetry-instrumentation-digma/pull/41
+        from .trace_decorator import instrument as _instrument
+
+        return _instrument
+    except Exception:  # nosec
+        print("Failed to import opentelemetry")
+        return noop
 
 
 instrument = setup_tracer()
```

### Comparing `syft-0.8.1b9/src/syft/util/trace_decorator.py` & `syft-0.8.2b1/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft/util/util.py` & `syft-0.8.2b1/src/syft/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,18 @@
 def get_name_for(klass: type):
     klass_name = getattr(klass, "__name__", None)
     if klass_name is None:
         klass_name = extract_name(klass)
     return klass_name
 
 
+def get_mb_size(data: Any) -> float:
+    return sys.getsizeof(data) / (1024 * 1024)
+
+
 def extract_name(klass: type):
     name_regex = r".+class.+?([\w\._]+).+"
     regex2 = r"([\w\.]+)"
     matches = re.match(name_regex, str(klass))
     if matches is None:
         matches = re.match(regex2, str(klass))
     try:
```

### Comparing `syft-0.8.1b9/src/syft/util/version_compare.py` & `syft-0.8.2b1/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b9/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b1/src/syft.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,134 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b9
+Version: 0.8.2b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: dev
+Provides-Extra: telemetry
 Provides-Extra: test_plugins
 Provides-Extra: oblv
 License-File: LICENSE
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/img/title_syft_dark.png">
   <img alt="Syft Logo" src="docs/img/title_syft_light.png" width="200px" />
 </picture>
 
-Perform `numpy`-like analysis on `data` that remains in `someone else's` server
+Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
-✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
+✅ `Linux` ✅ `macOS` ✅ `Windows`\* ✅ `Docker` ✅ `Kubernetes`
 
-## Install syft on Python 3.9 - 3.11
+## Install Client
 
 ```bash
 $ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
-## Launch a python dev Domain
+## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8,<0.8.1")
+sy.requires(">=0.8.1,<0.8.2")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
-## Connect with our Python Client
+## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8,<0.8.1")
+sy.requires(">=0.8.1,<0.8.2")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
+## PySyft in 10 minutes
+
+📝 <a href="/notebooks/api">API Example Notebooks</a>
+
+- <a href="/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+
+## Deploy Kubernetes Helm Chart
+
+```
+$ kubectl create namespace syft
+$ helm install my-domain syft --namespace syft --version 0.8.1 --repo https://openmined.github.io/PySyft/helm
+```
+
+### Azure or GCP Ingress
+
+```
+$ helm install ... --set ingress.ingressClass="azure/application-gateway"
+$ helm install ... --set ingress.ingressClass="gce"
+```
+
 ## Deploy to a Container Engine or Cloud
 
-1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server a one-liner:  
+1. Install our handy 🛵 cli tool which makes deploying a Domain or Gateway server to Docker or VM a one-liner:  
    `pip install -U hagrid`
 
 2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
    `hagrid quickstart`
 
 3. In the tutorial you will learn how to install and deploy:  
    `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`
 
    `PyGrid` = our 🐳 `docker` / 🐧 `vm` `Domain` & `Gateway` Servers where `private data` lives
 
-4. During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `podman` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†
-
 ## Docs and Support
 
-- 📝 <a href="/notebooks/api">API Example Notebooks</a>
 - 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
-- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
-  †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
-  \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
-  ‡`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
-- PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
+- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
+- PySyft 0.8.1 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
+  \*`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
+- PyGrid Requires: 🐳 `docker`, ☸️ `kubernetes` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
-`0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
-`0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
+`0.9.0` - Coming soon...  
+`0.8.2` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.1` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
 - `0.2.0` - `0.5.0`
 
 PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
 
@@ -126,14 +151,15 @@
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
 No more cold calls to get `access` to a dataset. No more weeks of `wait times` to get a `result` on your `query`. It also means `1000x more data` in every domain. PySyft opens the doors to a streamlined Data Scientist `workflow`, all with the individual's `privacy` at its heart.
 
+<!--
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
@@ -182,14 +208,15 @@
 - Deploy to GCP
 - Deploy to Kubernetes
 - Customize Networking
 - Modify PyGrid UI
 </td>
 </tr>
 </table>
+-->
 
 # Terminology
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
@@ -338,38 +365,53 @@
 <th align="center">
 <a href="https://opensource.fb.com/"><img src="docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
 <a href="https://pytorch.org/"><img src="docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="docs/img/logo_udacity.png" /></a>
+<a href="https://www.dpmc.govt.nz/">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_nz_dark.png">
+  <img src="docs/img/logo_nz_light.png" />
+</picture>
+</a>
+</th>
+<th align="center">
+<a href="https://twitter.com/"><img src="docs/img/logo_twitter.png" /></a>
+</th>
+<th align="center">
+<a href="https://google.com/"><img src="docs/img/logo_google.png" /></a>
+</th>
+<th align="center">
+<a href="https://microsoft.com/"><img src="docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://summerofcode.withgoogle.com/"><img src="docs/img/logo_gsoc.png" /></a>
+<a href="https://omidyar.com/"><img src="docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://developers.google.com/season-of-docs"><img src="docs/img/logo_gsod.png" /></a>
+<a href="https://www.udacity.com/"><img src="docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
+<a href="https://www.centerfordigitalhealthinnovation.org/">
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
-  <img src="docs/img/logo_arkhn_light.png" />
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cdhi_dark.png">
+  <img src="docs/img/logo_cdhi_light.png" />
 </picture>
 
+</a>
 </th>
 <th align="center">
+<a href="https://arkhn.org/">
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_cape.png">
-  <img src="docs/img/logo_cape_light.png" />
+  <source media="(prefers-color-scheme: dark)" srcset="docs/img/logo_arkhn.png">
+  <img src="docs/img/logo_arkhn_light.png" />
 </picture>
-</th>
-<th align="center">
-<a href="https://begin.ai/"><img src="docs/img/logo_begin.png" /></a>
+</a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
```

#### html2text {}

```diff
@@ -1,54 +1,58 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b9 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b1 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
-Provides-Extra: oblv License-File: LICENSE
+charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
+Provides-Extra: test_plugins Provides-Extra: oblv License-File: LICENSE
 [https://pepy.tech/badge/syft] [https://badge.fury.io/py/syft.svg] [https://
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
-  [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
-else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
-Install syft on Python 3.9 - 3.11 ```bash $ pip install -U syft -f https://
-whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
-Domain ```python # from Jupyter / Python import syft as sy sy.requires
-(">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
-dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
---name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
-8080 ``` ## Connect with our Python Client ```python import syft as sy
-sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
-email="info@openmined.org", password="changethis") ``` ## Deploy to a Container
-Engine or Cloud 1. Install our handy ðµ cli tool which makes deploying a
-Domain or Gateway server a one-liner: `pip install -U hagrid` 2. Then run our
+  [Syft Logo]  Perform data science on `data` that remains in `someone else's`
+server # Quickstart â `Linux` â `macOS` â `Windows`\* â `Docker` â
+`Kubernetes` ## Install Client ```bash $ pip install -U syft -f https://
+whls.blob.core.windows.net/unstable/index.html ``` ## Launch Server ```python #
+from Jupyter / Python import syft as sy sy.requires(">=0.8.1,<0.8.2") node =
+sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True) ```
+```bash # or from the command line $ syft launch --name=my-domain --port=8080 -
+-reset=True Starting syft-node server on 0.0.0.0:8080 ``` ## Launch Client
+```python import syft as sy sy.requires(">=0.8.1,<0.8.2") domain_client =
+sy.login(port=8080, email="info@openmined.org", password="changethis") ``` ##
+PySyft in 10 minutes ð API_Example_Notebooks - 00-load-data.ipynb - 01-
+submit-code.ipynb - 02-review-code-and-approve.ipynb - 03-data-scientist-
+download-result.ipynb - 04-jax-example.ipynb - 05-custom-policy.ipynb - 06-
+multiple-code-requests.ipynb - 07-domain-register-control-flow.ipynb ## Deploy
+Kubernetes Helm Chart ``` $ kubectl create namespace syft $ helm install my-
+domain syft --namespace syft --version 0.8.1 --repo https://
+openmined.github.io/PySyft/helm ``` ### Azure or GCP Ingress ``` $ helm install
+... --set ingress.ingressClass="azure/application-gateway" $ helm install ... -
+-set ingress.ingressClass="gce" ``` ## Deploy to a Container Engine or Cloud 1.
+Install our handy ðµ cli tool which makes deploying a Domain or Gateway
+server to Docker or VM a one-liner: `pip install -U hagrid` 2. Then run our
 interactive jupyter Install ð§ð½ââï¸ WizardBETA: `hagrid quickstart`
 3. In the tutorial you will learn how to install and deploy: `PySyft` = our
 `numpy`-like ð Python library for computing on `private data` in someone
 else's `Domain` `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway`
-Servers where `private data` lives 4. During quickstart we will deploy `PyGrid`
-to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
-a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
-`ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
-`#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
-`git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
-WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
-not support `ansible`, preventing some remote deployment targets - PySyft 0.8
-Requires: ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`macOS` Apple
-Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
+Servers where `private data` lives ## Docs and Support - ð Docs - `#support`
+on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run:
+`pip install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA
+Requires ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires:
+ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`Windows` users must
 run this first: `pip install jaxlib==0.4.10 -f https://
 whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
-`docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
-(Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
-- Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
+`docker`, â¸ï¸ `kubernetes` or ð§ `ubuntu` VM - Run: `hagrid launch ...` #
+Versions `0.9.0` - Coming soon... `0.8.2` (Beta) - `dev` branch ðð½ API -
+Coming soon... `0.8.1` (Stable) - API Deprecated: - `0.8.0` - API - `0.7.0` -
+Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
 context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
 ... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
 `hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
 version of `hagrid` is usually the best. # What is Syft?   [Syft]  `Syft` is
 OpenMined's `open source` stack that provides `secure` and `private` Data
@@ -66,27 +70,16 @@
 Data Science`. It means in a wide variety of `domains` across society, the
 current `risks` of sharing information (`copying` data) with someone such as,
 privacy invasion, IP theft and blackmail will no longer prevent the vast
 `benefits` such as innovation, insights and scientific discovery which secure
 access will provide. No more cold calls to get `access` to a dataset. No more
 weeks of `wait times` to get a `result` on your `query`. It also means `1000x
 more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Tutorials
- _____________________________________________________________________________
-|             [Image]     |            [Image]      |            [Image]      |
-|___________Data_Owner____|________Data_Scientist___|_________Data_Engineer___|
-|- Deploy_a_Domain_Server |- Install Syft           |- Setup Dev Mode         |
-|- Upload_Private_Data -  | - Connect to a Domain   | - Deploy to Azure -     |
-|Create_Accounts - Manage | - Search for Datasets   |Deploy to GCP - Deploy to|
-|Privacy Budget           | - Train Models -        |Kubernetes - Customize   |
-| - Join_a_Network - Learn|Retrieve Secure Results -|Networking - Modify      |
-|how PETs streamline Data |Learn Differential       |PyGrid UI                |
-|Policies_________________|Privacy__________________|_________________________|
-# Terminology
+Scientist `workflow`, all with the individual's `privacy` at its heart.  #
+Terminology
  _________________________________________________________________________________________
 |                 [Image]                  |                   [Image]                    |
 |_______ð¨ð»âð¼_Data|_______ð©ð½âð¬_Data_Sci|ntists
 | Provide `datasets` which they would like | Are end `users` who desire to perform        |
 |to make available for `study` by an       |`computations` or `answer` a specific         |
 |`outside party` they may or may not `fully|`question` using one or more data owners'     |
 |trust`_has_good_intentions._______________|`datasets`.___________________________________|
@@ -116,16 +109,16 @@
 # Courses
  _______________________
 |[Image]|[Image]|[Image]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
   [Contributors]  # Supporters
-  [docs/img/      [docs/img/     [docs/img/       [docs/img/       [docs/img/     [docs/img/         [docs/img/            [docs/img/       [docs/img/
-logo_sloan.png] logo_meta.png] logo_torch.png] logo_udacity.png] logo_gsoc.png] logo_gsod.png] logo_arkhn_light.png] logo_cape_light.png] logo_begin.png]
+  [docs/img/      [docs/img/     [docs/img/       __[docs/img/       [docs/img/        [docs/img/        [docs/img/       [docs/img/     [docs/img/         __[docs/img/         __[docs/img/
+logo_sloan.png] logo_meta.png] logo_torch.png] logo_nz_light.png] logo_twitter.png] logo_google.png] logo_microsoft.png] logo_on.png] logo_udacity.png] logo_cdhi_light.png] logo_arkhn_light.png]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on Open_Collective.
 
   [Contributors]  # Disclaimer Syft is under active development and is not yet
 ready for pilots on private data without our assistance. As early access
 participants, please contact us via [Slack](https://slack.openmined.org/) or
 email if you would like to ask a question or have a use case that you would
```

### Comparing `syft-0.8.1b9/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b1/src/syft.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 src/syft/external/oblv/deployment.py
 src/syft/external/oblv/deployment_client.py
 src/syft/external/oblv/exceptions.py
 src/syft/external/oblv/oblv_keys.py
 src/syft/external/oblv/oblv_keys_stash.py
 src/syft/external/oblv/oblv_proxy.py
 src/syft/external/oblv/oblv_service.py
+src/syft/img/base64.py
+src/syft/img/logo.png
+src/syft/img/small-grid-symbol-logo.png
 src/syft/node/__init__.py
 src/syft/node/credentials.py
 src/syft/node/domain.py
 src/syft/node/gateway.py
 src/syft/node/node.py
 src/syft/node/routes.py
 src/syft/node/run.py
@@ -148,18 +151,22 @@
 src/syft/types/syft_metaclass.py
 src/syft/types/syft_object.py
 src/syft/types/transforms.py
 src/syft/types/twin_object.py
 src/syft/types/uid.py
 src/syft/util/__init__.py
 src/syft/util/autoreload.py
+src/syft/util/colors.py
 src/syft/util/decorators.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
+src/syft/util/fonts.py
 src/syft/util/jax_settings.py
 src/syft/util/logger.py
 src/syft/util/markdown.py
+src/syft/util/options.py
 src/syft/util/schema.py
 src/syft/util/telemetry.py
 src/syft/util/trace_decorator.py
 src/syft/util/util.py
-src/syft/util/version_compare.py
+src/syft/util/version_compare.py
+src/syft/util/notebook_ui/notebook_addons.py
```

