# Comparing `tmp/cmon-ai-0.0.0.tar.gz` & `tmp/cmon-ai-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmon-ai-0.0.0.tar", last modified: Fri Jun 23 12:33:36 2023, max compression
+gzip compressed data, was "cmon-ai-0.2.6.tar", last modified: Fri Jun 23 12:34:06 2023, max compression
```

## Comparing `cmon-ai-0.0.0.tar` & `cmon-ai-0.2.6.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.260763 cmon-ai-0.0.0/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10826 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/LICENSE
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      218 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/MANIFEST.in
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15820 2023-06-23 12:33:36.260763 cmon-ai-0.0.0/PKG-INFO
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.212763 cmon-ai-0.0.0/Package_Installer/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      772 2023-06-23 12:16:36.000000 cmon-ai-0.0.0/Package_Installer/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      827 2023-06-23 11:39:42.000000 cmon-ai-0.0.0/Package_Installer/__main__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13830 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.212763 cmon-ai-0.0.0/cmon/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4701 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       69 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/__main__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      219 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/_docarray.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2794 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/checker.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.216763 cmon-ai-0.0.0/cmon/clients/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8347 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.216763 cmon-ai-0.0.0/cmon/clients/base/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7093 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11942 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    14582 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10197 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/http.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3760 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/retry.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2110 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/stream_rpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4227 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/unary_rpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9794 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/base/websocket.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2331 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2714 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2468 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/http.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    22535 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/mixin.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.216763 cmon-ai-0.0.0/cmon/clients/request/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3036 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/request/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2749 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/request/asyncio.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2748 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/request/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2443 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/clients/websocket.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2425 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/constants.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7782 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/enums.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5943 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/excepts.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2587 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/exporter.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    47518 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5996 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/importer.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.216763 cmon-ai-0.0.0/cmon/jaml/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    31248 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9313 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/jaml/parsers/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3249 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3169 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/base.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/jaml/parsers/deployment/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/deployment/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1922 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/deployment/legacy.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/jaml/parsers/executor/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/executor/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4515 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/executor/legacy.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/jaml/parsers/flow/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/flow/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6377 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/flow/v1.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/jaml/parsers/gateway/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/gateway/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2508 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/jaml/parsers/gateway/legacy.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/logging/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/logging/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2356 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/logging/formatter.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8318 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/logging/logger.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      113 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/logging/predefined.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8843 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/logging/profile.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/orchestrate/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/orchestrate/deployments/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    82370 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.220763 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    17751 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/docker_compose.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4560 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    15133 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8s.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.224763 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8slib/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8slib/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10662 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2914 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6916 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/deployments/install_requirements_helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.224763 cmon-ai-0.0.0/cmon/orchestrate/flow/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/flow/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2175 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/flow/asyncio.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)   145860 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/flow/base.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1704 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/flow/builder.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1144 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1800 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/orchestrator.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.224763 cmon-ai-0.0.0/cmon/orchestrate/pods/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12955 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/pods/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16580 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/pods/container.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2321 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/pods/container_helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1480 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/pods/factory.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2673 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/orchestrate/pods/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.228763 cmon-ai-0.0.0/cmon/parsers/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9433 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1322 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/base.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2520 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/client.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      574 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/create.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1108 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/deprecated.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3983 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/export.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1970 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/flow.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12817 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      505 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/logging.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.228763 cmon-ai-0.0.0/cmon/parsers/orchestrate/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5052 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/base.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2482 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/deployment.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9857 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/pod.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.228763 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3439 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/container.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      710 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/grpc_channel.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1228 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/head.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9107 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/remote.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1209 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/runtime.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4276 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/worker.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1489 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/parsers/ping.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.228763 cmon-ai-0.0.0/cmon/proto/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      227 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      457 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      477 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.228763 cmon-ai-0.0.0/cmon/proto/docarray_v1/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.232763 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9127 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.232763 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb2/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb2/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16512 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb2/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.232763 cmon-ai-0.0.0/cmon/proto/docarray_v2/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.232763 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9118 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.232763 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb2/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb2/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16503 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb2/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6906 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/proto/serializer.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.236763 cmon-ai-0.0.0/cmon/resources/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2327 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/Python.gitignore
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4170 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/ci-vendors.json
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3922 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/cmon.logo
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.236763 cmon-ai-0.0.0/cmon/resources/completions/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      567 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/completions/cmon.bash
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      663 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/completions/cmon.fish
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      425 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/completions/cmon.zsh
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3645 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/extra-requirements.txt
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.236763 cmon-ai-0.0.0/cmon/resources/health_check/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/health_check/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1500 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/health_check/gateway.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      672 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/health_check/pod.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.204763 cmon-ai-0.0.0/cmon/resources/k8s/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.240763 cmon-ai-0.0.0/cmon/resources/k8s/template/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      141 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/configmap.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2053 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-executor.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2061 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-gateway.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3357 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-uses-after.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4801 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-uses-before-after.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3367 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-uses-before.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      103 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/namespace.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      245 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/service.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      281 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/service_monitor.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      354 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/service_monitoring.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2459 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/k8s/template/statefulset-executor.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      886 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/logging.default.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      654 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/logging.docker.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      174 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/logging.json.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      431 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/logging.profile.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      673 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/logging.quiet.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      517 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/logging.remote.yml
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.204763 cmon-ai-0.0.0/cmon/resources/project-template/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.240763 cmon-ai-0.0.0/cmon/resources/project-template/deployment/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      176 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/deployment/client.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      120 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/deployment/deployment.yml
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.240763 cmon-ai-0.0.0/cmon/resources/project-template/deployment/executor1/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       45 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/deployment/executor1/config.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      225 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/deployment/executor1/executor.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/deployment/executor1/requirements.txt
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.240763 cmon-ai-0.0.0/cmon/resources/project-template/flow/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      176 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/flow/client.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.240763 cmon-ai-0.0.0/cmon/resources/project-template/flow/executor1/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       45 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/flow/executor1/config.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      225 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/flow/executor1/executor.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/flow/executor1/requirements.txt
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      163 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/resources/project-template/flow/flow.yml
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.244763 cmon-ai-0.0.0/cmon/schemas/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1111 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1057 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/deployment.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      111 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/executor.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1583 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/flow.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      320 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/gateway.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1639 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2415 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/schemas/meta.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.244763 cmon-ai-0.0.0/cmon/serve/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.244763 cmon-ai-0.0.0/cmon/serve/consensus/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2737 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/README.md
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2814 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/add_voter.go
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.244763 cmon-ai-0.0.0/cmon/serve/consensus/cmon-go-proto/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    68606 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon-go-proto/cmon.pb.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    36116 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8324 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon.proto
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.248763 cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3053 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/cmonraft.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      784 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/executor_connection.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11122 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/fsm.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4737 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/rpc.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3521 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/snapshot.go
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.248763 cmon-ai-0.0.0/cmon/serve/consensus/docarray-go-proto/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    42221 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/docarray-go-proto/docarray.pb.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2433 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/docarray.proto
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1004 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/go.mod
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    28154 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/go.sum
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2323 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/jraft.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2465 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/jraft.h
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    18360 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/run.go
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.248763 cmon-ai-0.0.0/cmon/serve/consensus/scripts/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      641 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/scripts/fetch-protos.sh
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1313 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/consensus/scripts/protogen.sh
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.248763 cmon-ai-0.0.0/cmon/serve/executors/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    51163 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/executors/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    20358 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/executors/decorators.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      928 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/executors/metas.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8398 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/executors/run.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6080 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.248763 cmon-ai-0.0.0/cmon/serve/instrumentation/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6869 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/instrumentation/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1739 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/monitoring.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.248763 cmon-ai-0.0.0/cmon/serve/networking/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    24332 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7628 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/connection_pool_map.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9399 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/connection_stub.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3094 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/instrumentation.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10258 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/replica_list.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13447 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/sse.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10504 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/networking/utils.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13845 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/asyncio.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10614 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/async_request_response_handling.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/composite/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      340 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/composite/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1650 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/gateway.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/graph/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/graph/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    32568 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/graph/topology_graph.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/grpc/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      306 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/grpc/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      732 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/health_model.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      416 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http/fastapi/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      347 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http/fastapi/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    17411 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http_fastapi_app.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9476 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/load_balancer/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      290 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/load_balancer/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10232 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/models.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11182 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/request_handling.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    20367 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/streamer.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/websocket/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      339 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/websocket/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12485 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/gateway/websocket_fastapi_app.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.252763 cmon-ai-0.0.0/cmon/serve/runtimes/head/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/head/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    24494 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/head/request_handling.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7742 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9296 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/monitoring.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.256763 cmon-ai-0.0.0/cmon/serve/runtimes/servers/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9783 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/servers/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3377 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/servers/composite.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8269 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/servers/grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9857 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/servers/http.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2255 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/servers/load_balancer.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4983 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/servers/websocket.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.256763 cmon-ai-0.0.0/cmon/serve/runtimes/worker/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/worker/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6088 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/worker/batch_queue.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6837 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/worker/http_fastapi_app.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    48714 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/runtimes/worker/request_handling.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.256763 cmon-ai-0.0.0/cmon/serve/stream/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13720 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/stream/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3505 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/serve/stream/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.256763 cmon-ai-0.0.0/cmon/types/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/types/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3814 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/types/mixin.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.256763 cmon-ai-0.0.0/cmon/types/request/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1631 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/types/request/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    14425 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/types/request/data.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2189 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon/types/request/status.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.256763 cmon-ai-0.0.0/cmon_ai.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15820 2023-06-23 12:33:36.000000 cmon-ai-0.0.0/cmon_ai.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8582 2023-06-23 12:33:36.000000 cmon-ai-0.0.0/cmon_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 12:33:36.000000 cmon-ai-0.0.0/cmon_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       39 2023-06-23 12:33:36.000000 cmon-ai-0.0.0/cmon_ai.egg-info/entry_points.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 12:32:29.000000 cmon-ai-0.0.0/cmon_ai.egg-info/not-zip-safe
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-06-23 12:33:36.000000 cmon-ai-0.0.0/cmon_ai.egg-info/top_level.txt
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:33:36.260763 cmon-ai-0.0.0/cmon_cli/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4210 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon_cli/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5173 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon_cli/api.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13006 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon_cli/autocomplete.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4165 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon_cli/export.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      193 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon_cli/known_plugins.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4719 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/cmon_cli/lookup.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3047 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/extra-requirements.txt
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4095 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/fastentrypoints.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       96 2023-06-23 09:57:47.000000 cmon-ai-0.0.0/pyproject.toml
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-06-23 12:33:36.260763 cmon-ai-0.0.0/setup.cfg
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8294 2023-06-23 12:31:56.000000 cmon-ai-0.0.0/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10826 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/LICENSE
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      218 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/MANIFEST.in
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15820 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/PKG-INFO
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.820762 cmon-ai-0.2.6/Package_Installer/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      772 2023-06-23 12:16:36.000000 cmon-ai-0.2.6/Package_Installer/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      827 2023-06-23 11:39:42.000000 cmon-ai-0.2.6/Package_Installer/__main__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13830 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.820762 cmon-ai-0.2.6/cmon/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4701 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       69 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/__main__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      219 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/_docarray.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2794 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/checker.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.824762 cmon-ai-0.2.6/cmon/clients/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8347 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.824762 cmon-ai-0.2.6/cmon/clients/base/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7093 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11942 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/grpc.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    14582 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10197 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/http.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3760 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/retry.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2110 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/stream_rpc.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4227 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/unary_rpc.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9794 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/base/websocket.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2331 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/grpc.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2714 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2468 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/http.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    22535 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/mixin.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.824762 cmon-ai-0.2.6/cmon/clients/request/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3036 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/request/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2749 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/request/asyncio.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2748 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/request/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2443 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/clients/websocket.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2425 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/constants.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7782 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/enums.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5943 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/excepts.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2587 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/exporter.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    47518 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5996 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/importer.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.824762 cmon-ai-0.2.6/cmon/jaml/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    31248 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9313 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/helper.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.824762 cmon-ai-0.2.6/cmon/jaml/parsers/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3249 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3169 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/base.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/jaml/parsers/deployment/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/deployment/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1922 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/deployment/legacy.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/jaml/parsers/executor/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/executor/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4515 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/executor/legacy.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/jaml/parsers/flow/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/flow/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6377 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/flow/v1.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/jaml/parsers/gateway/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/gateway/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2508 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/jaml/parsers/gateway/legacy.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/logging/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/logging/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2356 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/logging/formatter.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8318 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/logging/logger.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      113 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/logging/predefined.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8843 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/logging/profile.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/orchestrate/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.828762 cmon-ai-0.2.6/cmon/orchestrate/deployments/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    82370 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.832762 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    17751 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/docker_compose.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4560 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    15133 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8s.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.832762 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8slib/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8slib/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10662 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2914 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6916 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/deployments/install_requirements_helper.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.832762 cmon-ai-0.2.6/cmon/orchestrate/flow/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/flow/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2175 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/flow/asyncio.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)   145860 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/flow/base.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1704 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/flow/builder.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1144 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1800 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/orchestrator.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.832762 cmon-ai-0.2.6/cmon/orchestrate/pods/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12955 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/pods/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16580 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/pods/container.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2321 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/pods/container_helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1480 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/pods/factory.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2673 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/orchestrate/pods/helper.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.836762 cmon-ai-0.2.6/cmon/parsers/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9433 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1322 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/base.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2520 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/client.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      574 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/create.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1108 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/deprecated.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3983 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/export.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1970 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/flow.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12817 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      505 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/logging.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.836762 cmon-ai-0.2.6/cmon/parsers/orchestrate/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5052 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/base.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2482 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/deployment.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9857 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/pod.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.836762 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3439 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/container.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      710 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/grpc_channel.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1228 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/head.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9107 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/remote.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1209 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/runtime.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4276 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/worker.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1489 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/parsers/ping.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      227 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      457 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/cmon_pb2.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      477 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/cmon_pb2_grpc.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/docarray_v1/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9127 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb/cmon_pb2.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb2/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb2/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16512 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb2/cmon_pb2.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/docarray_v2/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9118 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb/cmon_pb2.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.840762 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb2/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb2/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16503 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb2/cmon_pb2.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6906 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/proto/serializer.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.844762 cmon-ai-0.2.6/cmon/resources/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2327 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/Python.gitignore
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4170 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/ci-vendors.json
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3922 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/cmon.logo
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.844762 cmon-ai-0.2.6/cmon/resources/completions/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      567 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/completions/cmon.bash
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      663 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/completions/cmon.fish
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      425 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/completions/cmon.zsh
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3645 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/extra-requirements.txt
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.844762 cmon-ai-0.2.6/cmon/resources/health_check/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/health_check/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1500 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/health_check/gateway.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      672 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/health_check/pod.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.812762 cmon-ai-0.2.6/cmon/resources/k8s/
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.848762 cmon-ai-0.2.6/cmon/resources/k8s/template/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      141 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/configmap.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2053 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-executor.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2061 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-gateway.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3357 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-uses-after.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4801 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-uses-before-after.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3367 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-uses-before.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      103 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/namespace.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      245 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/service.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      281 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/service_monitor.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      354 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/service_monitoring.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2459 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/k8s/template/statefulset-executor.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      886 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/logging.default.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      654 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/logging.docker.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      174 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/logging.json.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      431 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/logging.profile.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      673 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/logging.quiet.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      517 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/logging.remote.yml
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.812762 cmon-ai-0.2.6/cmon/resources/project-template/
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.848762 cmon-ai-0.2.6/cmon/resources/project-template/deployment/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      176 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/deployment/client.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      120 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/deployment/deployment.yml
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.848762 cmon-ai-0.2.6/cmon/resources/project-template/deployment/executor1/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       45 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/deployment/executor1/config.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      225 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/deployment/executor1/executor.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/deployment/executor1/requirements.txt
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.848762 cmon-ai-0.2.6/cmon/resources/project-template/flow/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      176 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/flow/client.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.848762 cmon-ai-0.2.6/cmon/resources/project-template/flow/executor1/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       45 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/flow/executor1/config.yml
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      225 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/flow/executor1/executor.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/flow/executor1/requirements.txt
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      163 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/resources/project-template/flow/flow.yml
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.852762 cmon-ai-0.2.6/cmon/schemas/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1111 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1057 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/deployment.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      111 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/executor.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1583 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/flow.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      320 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/gateway.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1639 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2415 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/schemas/meta.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.852762 cmon-ai-0.2.6/cmon/serve/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.852762 cmon-ai-0.2.6/cmon/serve/consensus/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2737 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/README.md
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2814 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/add_voter.go
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.852762 cmon-ai-0.2.6/cmon/serve/consensus/cmon-go-proto/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    68606 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon-go-proto/cmon.pb.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    36116 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8324 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon.proto
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.856762 cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3053 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/cmonraft.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      784 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/executor_connection.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11122 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/fsm.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4737 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/rpc.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3521 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/snapshot.go
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.856762 cmon-ai-0.2.6/cmon/serve/consensus/docarray-go-proto/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    42221 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/docarray-go-proto/docarray.pb.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2433 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/docarray.proto
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1004 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/go.mod
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    28154 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/go.sum
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2323 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/jraft.go
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2465 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/jraft.h
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    18360 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/run.go
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.856762 cmon-ai-0.2.6/cmon/serve/consensus/scripts/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      641 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/scripts/fetch-protos.sh
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1313 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/consensus/scripts/protogen.sh
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.856762 cmon-ai-0.2.6/cmon/serve/executors/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    51163 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/executors/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    20358 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/executors/decorators.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      928 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/executors/metas.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8398 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/executors/run.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6080 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/helper.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.856762 cmon-ai-0.2.6/cmon/serve/instrumentation/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6869 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/instrumentation/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1739 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/monitoring.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.860762 cmon-ai-0.2.6/cmon/serve/networking/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    24332 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7628 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/connection_pool_map.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9399 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/connection_stub.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3094 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/instrumentation.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10258 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/replica_list.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13447 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/sse.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10504 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/networking/utils.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.860762 cmon-ai-0.2.6/cmon/serve/runtimes/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13845 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/asyncio.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.860762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10614 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/async_request_response_handling.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.860762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/composite/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      340 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/composite/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1650 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/gateway.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/graph/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/graph/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    32568 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/graph/topology_graph.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/grpc/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      306 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/grpc/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      732 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/health_model.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      416 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http/__init__.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http/fastapi/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      347 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http/fastapi/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    17411 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http_fastapi_app.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9476 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/load_balancer/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      290 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/load_balancer/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10232 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/models.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11182 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/request_handling.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    20367 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/streamer.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/websocket/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      339 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/websocket/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12485 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/gateway/websocket_fastapi_app.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/head/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/head/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    24494 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/head/request_handling.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7742 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/helper.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9296 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/monitoring.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/servers/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9783 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/servers/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3377 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/servers/composite.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8269 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/servers/grpc.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9857 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/servers/http.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2255 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/servers/load_balancer.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4983 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/servers/websocket.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/runtimes/worker/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/worker/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6088 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/worker/batch_queue.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6837 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/worker/http_fastapi_app.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    48714 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/runtimes/worker/request_handling.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.864762 cmon-ai-0.2.6/cmon/serve/stream/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13720 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/stream/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3505 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/serve/stream/helper.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/cmon/types/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/types/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3814 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/types/mixin.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/cmon/types/request/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1631 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/types/request/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    14425 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/types/request/data.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2189 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon/types/request/status.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/cmon_ai.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15820 2023-06-23 12:34:06.000000 cmon-ai-0.2.6/cmon_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8582 2023-06-23 12:34:06.000000 cmon-ai-0.2.6/cmon_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 12:34:06.000000 cmon-ai-0.2.6/cmon_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       39 2023-06-23 12:34:06.000000 cmon-ai-0.2.6/cmon_ai.egg-info/entry_points.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 12:32:29.000000 cmon-ai-0.2.6/cmon_ai.egg-info/not-zip-safe
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-06-23 12:34:06.000000 cmon-ai-0.2.6/cmon_ai.egg-info/top_level.txt
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/cmon_cli/
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4210 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon_cli/__init__.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5173 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon_cli/api.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13006 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon_cli/autocomplete.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4165 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon_cli/export.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      193 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon_cli/known_plugins.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4719 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/cmon_cli/lookup.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3047 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/extra-requirements.txt
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4095 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/fastentrypoints.py
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       96 2023-06-23 09:57:47.000000 cmon-ai-0.2.6/pyproject.toml
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-06-23 12:34:06.868762 cmon-ai-0.2.6/setup.cfg
+-rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8294 2023-06-23 12:34:01.000000 cmon-ai-0.2.6/setup.py
```

### Comparing `cmon-ai-0.0.0/LICENSE` & `cmon-ai-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/PKG-INFO` & `cmon-ai-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmon-ai
-Version: 0.0.0
+Version: 0.2.6
 Summary: Build multimodal AI services via cloud native technologies · Neural Search · Generative AI · MLOps
 Home-page: https://github.com/alinooriyan/Cmon-AI
 Download-URL: https://github.com/alinooriyan/Cmon-AI/archive/refs/tags/AI.zip
 Author: Cmon AI
 Author-email: hello@cmon.ai
 License: Apache 2.0
 Project-URL: Documentation, https://docs.cmon.pw
```

### Comparing `cmon-ai-0.0.0/Package_Installer/__init__.py` & `cmon-ai-0.2.6/Package_Installer/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/Package_Installer/__main__.py` & `cmon-ai-0.2.6/Package_Installer/__main__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/README.md` & `cmon-ai-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/__init__.py` & `cmon-ai-0.2.6/cmon/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/checker.py` & `cmon-ai-0.2.6/cmon/checker.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/__init__.py` & `cmon-ai-0.2.6/cmon/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/__init__.py` & `cmon-ai-0.2.6/cmon/clients/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/grpc.py` & `cmon-ai-0.2.6/cmon/clients/base/grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/helper.py` & `cmon-ai-0.2.6/cmon/clients/base/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/http.py` & `cmon-ai-0.2.6/cmon/clients/base/http.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/retry.py` & `cmon-ai-0.2.6/cmon/clients/base/retry.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/stream_rpc.py` & `cmon-ai-0.2.6/cmon/clients/base/stream_rpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/unary_rpc.py` & `cmon-ai-0.2.6/cmon/clients/base/unary_rpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/base/websocket.py` & `cmon-ai-0.2.6/cmon/clients/base/websocket.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/grpc.py` & `cmon-ai-0.2.6/cmon/clients/grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/helper.py` & `cmon-ai-0.2.6/cmon/clients/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/http.py` & `cmon-ai-0.2.6/cmon/clients/http.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/mixin.py` & `cmon-ai-0.2.6/cmon/clients/mixin.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/request/__init__.py` & `cmon-ai-0.2.6/cmon/clients/request/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/request/asyncio.py` & `cmon-ai-0.2.6/cmon/clients/request/asyncio.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/request/helper.py` & `cmon-ai-0.2.6/cmon/clients/request/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/clients/websocket.py` & `cmon-ai-0.2.6/cmon/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/constants.py` & `cmon-ai-0.2.6/cmon/constants.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/enums.py` & `cmon-ai-0.2.6/cmon/enums.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/excepts.py` & `cmon-ai-0.2.6/cmon/excepts.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/exporter.py` & `cmon-ai-0.2.6/cmon/exporter.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/helper.py` & `cmon-ai-0.2.6/cmon/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/importer.py` & `cmon-ai-0.2.6/cmon/importer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/__init__.py` & `cmon-ai-0.2.6/cmon/jaml/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/helper.py` & `cmon-ai-0.2.6/cmon/jaml/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/parsers/__init__.py` & `cmon-ai-0.2.6/cmon/jaml/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/parsers/base.py` & `cmon-ai-0.2.6/cmon/jaml/parsers/base.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/parsers/deployment/legacy.py` & `cmon-ai-0.2.6/cmon/jaml/parsers/deployment/legacy.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/parsers/executor/legacy.py` & `cmon-ai-0.2.6/cmon/jaml/parsers/executor/legacy.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/parsers/flow/v1.py` & `cmon-ai-0.2.6/cmon/jaml/parsers/flow/v1.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/jaml/parsers/gateway/legacy.py` & `cmon-ai-0.2.6/cmon/jaml/parsers/gateway/legacy.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/logging/formatter.py` & `cmon-ai-0.2.6/cmon/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/logging/logger.py` & `cmon-ai-0.2.6/cmon/logging/logger.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/logging/profile.py` & `cmon-ai-0.2.6/cmon/logging/profile.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/__init__.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/config/docker_compose.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/config/docker_compose.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/config/helper.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/config/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8s.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8s.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/deployments/install_requirements_helper.py` & `cmon-ai-0.2.6/cmon/orchestrate/deployments/install_requirements_helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/flow/asyncio.py` & `cmon-ai-0.2.6/cmon/orchestrate/flow/asyncio.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/flow/base.py` & `cmon-ai-0.2.6/cmon/orchestrate/flow/base.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/flow/builder.py` & `cmon-ai-0.2.6/cmon/orchestrate/flow/builder.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/helper.py` & `cmon-ai-0.2.6/cmon/orchestrate/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/orchestrator.py` & `cmon-ai-0.2.6/cmon/orchestrate/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/pods/__init__.py` & `cmon-ai-0.2.6/cmon/orchestrate/pods/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/pods/container.py` & `cmon-ai-0.2.6/cmon/orchestrate/pods/container.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/pods/container_helper.py` & `cmon-ai-0.2.6/cmon/orchestrate/pods/container_helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/pods/factory.py` & `cmon-ai-0.2.6/cmon/orchestrate/pods/factory.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/orchestrate/pods/helper.py` & `cmon-ai-0.2.6/cmon/orchestrate/pods/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/__init__.py` & `cmon-ai-0.2.6/cmon/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/base.py` & `cmon-ai-0.2.6/cmon/parsers/base.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/client.py` & `cmon-ai-0.2.6/cmon/parsers/client.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/create.py` & `cmon-ai-0.2.6/cmon/parsers/create.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/deprecated.py` & `cmon-ai-0.2.6/cmon/parsers/deprecated.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/export.py` & `cmon-ai-0.2.6/cmon/parsers/export.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/flow.py` & `cmon-ai-0.2.6/cmon/parsers/flow.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/helper.py` & `cmon-ai-0.2.6/cmon/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/base.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/base.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/deployment.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/deployment.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/pod.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/pod.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/container.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/container.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/grpc_channel.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/grpc_channel.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/head.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/head.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/remote.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/remote.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/runtime.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/runtime.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/orchestrate/runtimes/worker.py` & `cmon-ai-0.2.6/cmon/parsers/orchestrate/runtimes/worker.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/parsers/ping.py` & `cmon-ai-0.2.6/cmon/parsers/ping.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v1/pb/cmon_pb2.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v1/pb/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v1/pb2/cmon_pb2.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v1/pb2/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v2/pb/cmon_pb2.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v2/pb/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v2/pb2/cmon_pb2.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v2/pb2/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py` & `cmon-ai-0.2.6/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/proto/serializer.py` & `cmon-ai-0.2.6/cmon/proto/serializer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/Python.gitignore` & `cmon-ai-0.2.6/cmon/resources/Python.gitignore`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/ci-vendors.json` & `cmon-ai-0.2.6/cmon/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/cmon.logo` & `cmon-ai-0.2.6/cmon/resources/cmon.logo`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/completions/cmon.bash` & `cmon-ai-0.2.6/cmon/resources/completions/cmon.bash`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/completions/cmon.fish` & `cmon-ai-0.2.6/cmon/resources/completions/cmon.fish`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/extra-requirements.txt` & `cmon-ai-0.2.6/cmon/resources/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/health_check/gateway.py` & `cmon-ai-0.2.6/cmon/resources/health_check/gateway.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/health_check/pod.py` & `cmon-ai-0.2.6/cmon/resources/health_check/pod.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-executor.yml` & `cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-executor.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-gateway.yml` & `cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-gateway.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-uses-after.yml` & `cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-uses-after.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-uses-before-after.yml` & `cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-uses-before-after.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/k8s/template/deployment-uses-before.yml` & `cmon-ai-0.2.6/cmon/resources/k8s/template/deployment-uses-before.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/k8s/template/statefulset-executor.yml` & `cmon-ai-0.2.6/cmon/resources/k8s/template/statefulset-executor.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/logging.default.yml` & `cmon-ai-0.2.6/cmon/resources/logging.default.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/logging.docker.yml` & `cmon-ai-0.2.6/cmon/resources/logging.docker.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/logging.quiet.yml` & `cmon-ai-0.2.6/cmon/resources/logging.quiet.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/resources/logging.remote.yml` & `cmon-ai-0.2.6/cmon/resources/logging.remote.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/schemas/__init__.py` & `cmon-ai-0.2.6/cmon/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/schemas/deployment.py` & `cmon-ai-0.2.6/cmon/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/schemas/flow.py` & `cmon-ai-0.2.6/cmon/schemas/flow.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/schemas/helper.py` & `cmon-ai-0.2.6/cmon/schemas/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/schemas/meta.py` & `cmon-ai-0.2.6/cmon/schemas/meta.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/README.md` & `cmon-ai-0.2.6/cmon/serve/consensus/README.md`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/add_voter.go` & `cmon-ai-0.2.6/cmon/serve/consensus/add_voter.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon-go-proto/cmon.pb.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon-go-proto/cmon.pb.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon.proto` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon.proto`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/cmonraft.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/cmonraft.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/executor_connection.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/executor_connection.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/fsm.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/fsm.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/rpc.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/rpc.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/cmon_raft/snapshot.go` & `cmon-ai-0.2.6/cmon/serve/consensus/cmon_raft/snapshot.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/docarray-go-proto/docarray.pb.go` & `cmon-ai-0.2.6/cmon/serve/consensus/docarray-go-proto/docarray.pb.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/docarray.proto` & `cmon-ai-0.2.6/cmon/serve/consensus/docarray.proto`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/go.mod` & `cmon-ai-0.2.6/cmon/serve/consensus/go.mod`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/go.sum` & `cmon-ai-0.2.6/cmon/serve/consensus/go.sum`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/jraft.go` & `cmon-ai-0.2.6/cmon/serve/consensus/jraft.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/jraft.h` & `cmon-ai-0.2.6/cmon/serve/consensus/jraft.h`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/run.go` & `cmon-ai-0.2.6/cmon/serve/consensus/run.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/scripts/fetch-protos.sh` & `cmon-ai-0.2.6/cmon/serve/consensus/scripts/fetch-protos.sh`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/consensus/scripts/protogen.sh` & `cmon-ai-0.2.6/cmon/serve/consensus/scripts/protogen.sh`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/executors/__init__.py` & `cmon-ai-0.2.6/cmon/serve/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/executors/decorators.py` & `cmon-ai-0.2.6/cmon/serve/executors/decorators.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/executors/metas.py` & `cmon-ai-0.2.6/cmon/serve/executors/metas.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/executors/run.py` & `cmon-ai-0.2.6/cmon/serve/executors/run.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/helper.py` & `cmon-ai-0.2.6/cmon/serve/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/instrumentation/__init__.py` & `cmon-ai-0.2.6/cmon/serve/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/monitoring.py` & `cmon-ai-0.2.6/cmon/serve/monitoring.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/__init__.py` & `cmon-ai-0.2.6/cmon/serve/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/connection_pool_map.py` & `cmon-ai-0.2.6/cmon/serve/networking/connection_pool_map.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/connection_stub.py` & `cmon-ai-0.2.6/cmon/serve/networking/connection_stub.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/instrumentation.py` & `cmon-ai-0.2.6/cmon/serve/networking/instrumentation.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/replica_list.py` & `cmon-ai-0.2.6/cmon/serve/networking/replica_list.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/sse.py` & `cmon-ai-0.2.6/cmon/serve/networking/sse.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/networking/utils.py` & `cmon-ai-0.2.6/cmon/serve/networking/utils.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/asyncio.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/asyncio.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/async_request_response_handling.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/async_request_response_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/gateway.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/graph/topology_graph.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/graph/topology_graph.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/health_model.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/health_model.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http_fastapi_app.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http_fastapi_app.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/models.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/models.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/request_handling.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/request_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/streamer.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/streamer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/gateway/websocket_fastapi_app.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/gateway/websocket_fastapi_app.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/head/request_handling.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/head/request_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/helper.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/monitoring.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/monitoring.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/servers/__init__.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/servers/composite.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/servers/composite.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/servers/grpc.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/servers/grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/servers/http.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/servers/http.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/servers/load_balancer.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/servers/load_balancer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/servers/websocket.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/servers/websocket.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/worker/batch_queue.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/worker/batch_queue.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/worker/http_fastapi_app.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/worker/http_fastapi_app.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/runtimes/worker/request_handling.py` & `cmon-ai-0.2.6/cmon/serve/runtimes/worker/request_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/stream/__init__.py` & `cmon-ai-0.2.6/cmon/serve/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/serve/stream/helper.py` & `cmon-ai-0.2.6/cmon/serve/stream/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/types/mixin.py` & `cmon-ai-0.2.6/cmon/types/mixin.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/types/request/__init__.py` & `cmon-ai-0.2.6/cmon/types/request/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/types/request/data.py` & `cmon-ai-0.2.6/cmon/types/request/data.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon/types/request/status.py` & `cmon-ai-0.2.6/cmon/types/request/status.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon_ai.egg-info/PKG-INFO` & `cmon-ai-0.2.6/cmon_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmon-ai
-Version: 0.0.0
+Version: 0.2.6
 Summary: Build multimodal AI services via cloud native technologies · Neural Search · Generative AI · MLOps
 Home-page: https://github.com/alinooriyan/Cmon-AI
 Download-URL: https://github.com/alinooriyan/Cmon-AI/archive/refs/tags/AI.zip
 Author: Cmon AI
 Author-email: hello@cmon.ai
 License: Apache 2.0
 Project-URL: Documentation, https://docs.cmon.pw
```

### Comparing `cmon-ai-0.0.0/cmon_ai.egg-info/SOURCES.txt` & `cmon-ai-0.2.6/cmon_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon_cli/__init__.py` & `cmon-ai-0.2.6/cmon_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon_cli/api.py` & `cmon-ai-0.2.6/cmon_cli/api.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon_cli/autocomplete.py` & `cmon-ai-0.2.6/cmon_cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon_cli/export.py` & `cmon-ai-0.2.6/cmon_cli/export.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/cmon_cli/lookup.py` & `cmon-ai-0.2.6/cmon_cli/lookup.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/extra-requirements.txt` & `cmon-ai-0.2.6/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/fastentrypoints.py` & `cmon-ai-0.2.6/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.0.0/setup.py` & `cmon-ai-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     libinfo_py = path.join(pkg_name, '__init__.py')
     libinfo_content = open(libinfo_py, 'r', encoding='utf-8').readlines()
     version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][
         0
     ]
     exec(version_line)  # gives __version__
 except FileNotFoundError:
-    __version__ = '0.0.0'
+    __version__ = '0.2.6'
 
 try:
     with open('README.md', encoding='utf-8') as fp:
         _long_description = fp.read()
 except FileNotFoundError:
     _long_description = ''
```

