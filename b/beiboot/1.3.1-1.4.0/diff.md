# Comparing `tmp/beiboot-1.3.1.tar.gz` & `tmp/beiboot-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beiboot-1.3.1.tar", max compression
+gzip compressed data, was "beiboot-1.4.0.tar", max compression
```

## Comparing `beiboot-1.3.1.tar` & `beiboot-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0      699 2023-01-24 09:41:20.255643 beiboot-1.3.1/README.md
--rw-r--r--   0        0        0        0 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/__init__.py
--rw-r--r--   0        0        0      180 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/__init__.py
--rw-r--r--   0        0        0     2424 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/connect.py
--rw-r--r--   0        0        0     2199 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/create.py
--rw-r--r--   0        0        0     1558 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/delete.py
--rw-r--r--   0        0        0     1977 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/heartbeat.py
--rw-r--r--   0        0        0     1335 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/list.py
--rw-r--r--   0        0        0      993 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/read.py
--rw-r--r--   0        0        0      390 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/api/utils.py
--rw-r--r--   0        0        0     3441 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/configuration.py
--rw-r--r--   0        0        0        0 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/__init__.py
--rw-r--r--   0        0        0     4217 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/abstract.py
--rw-r--r--   0        0        0     1914 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/dummy/__init__.py
--rw-r--r--   0        0        0     1285 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/factory.py
--rw-r--r--   0        0        0       52 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/ghostunnel/__init__.py
--rw-r--r--   0        0        0     5854 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/ghostunnel/docker.py
--rw-r--r--   0        0        0       65 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/ghostunnel/native.py
--rw-r--r--   0        0        0      137 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/types.py
--rw-r--r--   0        0        0      555 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/connection/utils.py
--rw-r--r--   0        0        0        0 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/__init__.py
--rw-r--r--   0        0        0      218 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/comps/__init__.py
--rw-r--r--   0        0        0     1657 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/comps/configmap.py
--rw-r--r--   0        0        0     1179 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/comps/deployment.py
--rw-r--r--   0        0        0      262 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/comps/namespace.py
--rw-r--r--   0        0        0     3019 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/comps/rbac.py
--rw-r--r--   0        0        0     4326 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/comps/webhook.py
--rw-r--r--   0        0        0     1626 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/install.py
--rw-r--r--   0        0        0     3561 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/uninstall.py
--rw-r--r--   0        0        0      481 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/misc/utils.py
--rw-r--r--   0        0        0    14464 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/types.py
--rw-r--r--   0        0        0     4013 2023-01-24 09:41:20.255643 beiboot-1.3.1/beiboot/utils.py
--rw-r--r--   0        0        0     1397 2023-01-24 09:41:20.255643 beiboot-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1654 1970-01-01 00:00:00.000000 beiboot-1.3.1/setup.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 beiboot-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      699 2023-06-23 09:24:29.427409 beiboot-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/connect.py
+-rw-r--r--   0        0        0     2199 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/create.py
+-rw-r--r--   0        0        0     2256 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/create_shelf.py
+-rw-r--r--   0        0        0     1558 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/delete.py
+-rw-r--r--   0        0        0     1535 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/delete_shelf.py
+-rw-r--r--   0        0        0     1977 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/heartbeat.py
+-rw-r--r--   0        0        0     1335 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/list.py
+-rw-r--r--   0        0        0     1335 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/list_shelves.py
+-rw-r--r--   0        0        0      993 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/read.py
+-rw-r--r--   0        0        0      995 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/read_shelf.py
+-rw-r--r--   0        0        0      390 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/api/utils.py
+-rw-r--r--   0        0        0     3441 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/configuration.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/__init__.py
+-rw-r--r--   0        0        0     4217 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/abstract.py
+-rw-r--r--   0        0        0     1914 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/dummy/__init__.py
+-rw-r--r--   0        0        0     1285 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/factory.py
+-rw-r--r--   0        0        0       52 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/ghostunnel/__init__.py
+-rw-r--r--   0        0        0     5854 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/ghostunnel/docker.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/ghostunnel/native.py
+-rw-r--r--   0        0        0      137 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/types.py
+-rw-r--r--   0        0        0      555 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/connection/utils.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/__init__.py
+-rw-r--r--   0        0        0      218 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/comps/__init__.py
+-rw-r--r--   0        0        0     1689 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/comps/configmap.py
+-rw-r--r--   0        0        0     1179 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/comps/deployment.py
+-rw-r--r--   0        0        0      262 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/comps/namespace.py
+-rw-r--r--   0        0        0     3582 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/comps/rbac.py
+-rw-r--r--   0        0        0     8194 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/comps/webhook.py
+-rw-r--r--   0        0        0     1626 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/install.py
+-rw-r--r--   0        0        0     3856 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/uninstall.py
+-rw-r--r--   0        0        0      481 2023-06-23 09:24:29.427409 beiboot-1.4.0/beiboot/misc/utils.py
+-rw-r--r--   0        0        0    17952 2023-06-23 09:24:29.431409 beiboot-1.4.0/beiboot/types.py
+-rw-r--r--   0        0        0     4665 2023-06-23 09:24:29.431409 beiboot-1.4.0/beiboot/utils.py
+-rw-r--r--   0        0        0     1750 2023-06-23 09:24:29.431409 beiboot-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 beiboot-1.4.0/PKG-INFO
```

### Comparing `beiboot-1.3.1/README.md` & `beiboot-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/api/connect.py` & `beiboot-1.4.0/beiboot/api/connect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
-from typing import Optional
+from typing import Optional, List
 
 from beiboot.api.utils import stopwatch
 from beiboot.configuration import default_configuration, ClientConfiguration
 from beiboot.connection.abstract import AbstractConnector
 from beiboot.connection.factory import connector_factory
 from beiboot.connection.types import ConnectorType
-from beiboot.types import Beiboot, BeibootProvider
+from beiboot.types import Beiboot
 
 logger = logging.getLogger(__name__)
 
 
 def _get_connector(
     connector_type: ConnectorType, config: ClientConfiguration
 ) -> AbstractConnector:
@@ -38,17 +38,15 @@
     :type connector_type: ConnectorType
     :param host: The host to connect to.
     :param config: The client configuration to use.
     :type config: ClientConfiguration
 
     :return: A AbstractConnector instance
     """
-    additional_ports = []
-    if BeibootProvider(beiboot.provider) == BeibootProvider.K3S:
-        additional_ports = ["6443:6443"]
+    additional_ports: List = []
     connector = _get_connector(connector_type, config)
 
     if connector_type == ConnectorType.GHOSTUNNEL_DOCKER and _docker_network:
         # this is for local testing purposes
         connector.set_docker_network(_docker_network)  # type: ignore
 
     connector.establish(beiboot, additional_ports, host)
```

### Comparing `beiboot-1.3.1/beiboot/api/create.py` & `beiboot-1.4.0/beiboot/api/create.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/api/delete.py` & `beiboot-1.4.0/beiboot/api/delete.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/api/heartbeat.py` & `beiboot-1.4.0/beiboot/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/api/list.py` & `beiboot-1.4.0/beiboot/api/list.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/api/read.py` & `beiboot-1.4.0/beiboot/api/read.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/configuration.py` & `beiboot-1.4.0/beiboot/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger(__name__)
 logger.addHandler(console)
 
-__VERSION__ = "1.3.1"
+__VERSION__ = "1.4.0"
 
 
 class ClientConfiguration(object):
     def __init__(
         self,
         getdeck_config_root: Optional[Union[str, Path]] = None,
         docker_client=None,
```

### Comparing `beiboot-1.3.1/beiboot/connection/abstract.py` & `beiboot-1.4.0/beiboot/connection/abstract.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/connection/dummy/__init__.py` & `beiboot-1.4.0/beiboot/connection/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/connection/factory.py` & `beiboot-1.4.0/beiboot/connection/factory.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/connection/ghostunnel/docker.py` & `beiboot-1.4.0/beiboot/connection/ghostunnel/docker.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/connection/utils.py` & `beiboot-1.4.0/beiboot/connection/utils.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/misc/comps/configmap.py` & `beiboot-1.4.0/beiboot/misc/comps/configmap.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,20 +13,20 @@
             "data": {
                 "clusterReadyTimeout": "180",
                 "gefyra": '{"enabled": true, "endpoint": null}',
                 "k8sVersion": "null",
                 "maxLifetime": params.max_lifetime,
                 "maxSessionTimeout": params.max_session_timeout,
                 "namespacePrefix": params.namespace_prefix,
-                "nodeLabels": '{"app": "beiboot", "beiboot.dev/is-node": "true"}',
+                "nodeLabels": '{"app": "beiboot", "beiboot.getdeck.dev/is-node": "true"}',
                 "nodeResources": f'{{"requests": {{"cpu": "{params.node_requests_cpu}", "memory": "{params.node_requests_memory}"}}, "limits": {{}}}}',  # noqa
                 "nodeStorageRequests": params.node_storage_request,
                 "nodes": params.nodes,
                 "ports": "null",
-                "serverLabels": '{"app": "beiboot", "beiboot.dev/is-node": "true", "beiboot.dev/is-server": "true"}',
+                "serverLabels": '{"app": "beiboot", "beiboot.getdeck.dev/is-node": "true", "beiboot.getdeck.dev/is-server": "true"}',  # noqa
                 "serverResources": f'{{"requests": {{"cpu": "{params.server_requests_cpu}", "memory": "{params.server_requests_memory}"}}, "limits": {{}}}}',  # noqa
                 "serverStartupTimeout": "60",
                 "serverStorageRequests": params.server_storage_request,
                 "tunnel": '{"enabled": true, "endpoint": null}',
                 "storageClass": params.storage_class,
                 "shelfStorageClass": params.shelf_storage_class,
             },
```

### Comparing `beiboot-1.3.1/beiboot/misc/comps/deployment.py` & `beiboot-1.4.0/beiboot/misc/comps/deployment.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/misc/comps/rbac.py` & `beiboot-1.4.0/beiboot/misc/comps/rbac.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,26 +47,41 @@
                         "serviceaccounts",
                         "rolebindings",
                         "nodes",
                         "configmaps",
                         "secrets",
                         "deployments",
                         "statefulsets",
+                        "persistentvolumeclaims",
                         "services",
                         "pods",
                         "pods/exec",
                         "events",
                     ],
                     "verbs": ["*"],
                 },
                 {
                     "apiGroups": ["getdeck.dev"],
                     "resources": ["beiboots"],
                     "verbs": ["*"],
                 },
+                {
+                    "apiGroups": ["beiboots.getdeck.dev"],
+                    "resources": ["shelves"],
+                    "verbs": ["*"],
+                },
+                {
+                    "apiGroups": ["snapshot.storage.k8s.io"],
+                    "resources": [
+                        "volumesnapshots",
+                        "volumesnapshotcontents",
+                        "volumesnapshotclasses",
+                    ],
+                    "verbs": ["*"],
+                },
             ],
         },
         {
             "apiVersion": "rbac.authorization.k8s.io/v1",
             "kind": "ClusterRoleBinding",
             "metadata": {
                 "name": "getdeck-beiboot-operator",
```

### Comparing `beiboot-1.3.1/beiboot/misc/comps/webhook.py` & `beiboot-1.4.0/beiboot/misc/comps/webhook.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,8 +43,42 @@
                         }
                     ],
                     "sideEffects": "None",
                     "timeoutSeconds": 30,
                 }
             ],
         },
+        {
+            "apiVersion": "admissionregistration.k8s.io/v1",
+            "kind": "ValidatingWebhookConfiguration",
+            "metadata": {"name": "shelf.beiboots.getdeck.dev"},
+            "webhooks": [
+                {
+                    "admissionReviewVersions": ["v1", "v1beta1"],
+                    "clientConfig": {
+                        "caBundle": "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUZDakNDQXZLZ0F3SUJBZ0lVTzJZMlJqUVdL\nVi9yTkJpOUx5Ry9xVWFqWENBd0RRWUpLb1pJaHZjTkFRRUwKQlFBd0tERW1NQ1FHQTFVRUF3d2RZ\nbVZwWW05dmRDMWhaRzFwYzNOcGIyNHVaMlYwWkdWamF5NXpkbU13SGhjTgpNakl4TVRFNE1qRXlO\nelUyV2hjTk1qTXhNVEU0TWpFeU56VTJXakFvTVNZd0pBWURWUVFEREIxaVpXbGliMjkwCkxXRmti\nV2x6YzJsdmJpNW5aWFJrWldOckxuTjJZekNDQWlJd0RRWUpLb1pJaHZjTkFRRUJCUUFEZ2dJUEFE\nQ0MKQWdvQ2dnSUJBTFd6OWc1dDdkbVN4dm9ob1hvSHRnQWsvdEpiOTlKLzNoekdzSGgwWExYbTBs\nbXJ3LzAvUjd4dworcXJPajdreUZ4R1NUREY0MGRmNyt5S3VTdkZxNGhpQjlqaFppakNTOFF4SFZ1\nTFVtMGNydjZGYWtKVmNVVW1DClZvRmkvNlJCVktLS0p4TzlRUU1YMWtaeUNXaW1wblN6d2Y0NDM5\nd0U0ZTJVcXBpWXl6Q2ZNZmlzQWVLRDE1dnQKYmRvM0NFYTVhc2tRTnFvZ0xYUWNxL0pkOTROYzN2\nQ2lVbGxUVXRJZkovb0VxS05tbmFqaHBRTVEwZ1plY0dESwo0SnZhcnNSd3I3N0RKUWllUWJsRi9w\naW0xcjQ2UGQzQk1DSHVMUVNrdERxdTNFK1BHZkNLZC95SmhKQVhUTmorClZqdGxUZGYxZm5MS0hM\nU1Qyck9MK3lzZVR1WnA4eGtEQnZNcmlCajg0RDVZeEVQNUIwZm9rVTM2UUZJMkdydFcKNjFPZjNN\nN1l4V3dFbHBhYUJnRFk5MDQvNU5TcE5WVFJBYVdZZHZDUmdnOC91Qmw2NXR1MGQ3d21jamlRK1Fm\nZQptRHhQczN0T29QMUZOcnYwUDk2dnRSVE55WGNVSXNUaWl4eDdQSjBkUnlINGdQdy92ZFluUElh\nRWFXOEpQaWI2CllVaVJHeFFWaXZLaDJ1NW1QaHlodzRxT3VNVHU5c1pIYjc4cEtpMGtsRko1TDNX\nWlNRUmFIUUZwRitVQncyclgKVDgzZjAxaDZXMlY3dm00TVNtRzBqcEYwdDM3cU1WUmNxVXpjeTFt\nUUVKVFFrck0rSVd1cGQ5V2d0cmhHc2M5RApvUXpGSTFIRm5mTGVMVXVUeVkrOVpNR25PcGlKVnNk\nMDNjMzJ0ay95SVcrbUZOTE8xbnJCQWdNQkFBR2pMREFxCk1DZ0dBMVVkRVFRaE1CK0NIV0psYVdK\ndmIzUXRZV1J0YVhOemFXOXVMbWRsZEdSbFkyc3VjM1pqTUEwR0NTcUcKU0liM0RRRUJDd1VBQTRJ\nQ0FRQ2JxQWJOT0hlUmdwbTloVmVSSDIxVHg1c2hmbEpzOU0vQy9iMDV2TUFWQjZiRgpBRktyNndT\nRDcwMk1yWFd4SG00SlZBY01xZVFvODlzb2J1S0FtUWd5WTdNdlllSnJHWjBrT0htZzRKZVcxTnFU\nCmhQUGRqNXdaZ05WcHg0dXl5NG9NK05pVW5CTndVS0diK2F0MGwxSmVLWUlwR1lySmtSQlo0ZmRk\nWlFvYU0yY1gKUmM1OWxCSisraVA2SnBuNGdKR2l2UEZwOGdTczFkanBUTWRWU3VJelJkbzlmNU81\nNEt6WnJ0di9ITzM5aVB6QQpSWnVNYlFzOU0zUDZObkQ0c3JSTjlQcG1KUXpuM1RSYlFUeDBoRkpw\nTmN0L1FkKzUyRzM1Tk81Zy9tVUk5aHowCjNRSy9rMlVSMUtMZ24ycURjMk4zanhjT1R2YURDbEVZ\nSDFnOVlMTnVuMU4rVzdLeUNwUzNlazhkZkgzeTRLNVQKZnUrT01VQjFRaDJJbWV3RzJTVnpFTmRE\nYjFxenMxellhYXlGVmFsalJEeW5MclJrTlUzWEo2WTlkMlM3NmllbApvZWtiT1N5RGtRdThHUllx\nQzNGckVROUN3STd5RFp1RnVoZnZGWTdrNzcvL3VuVDRHTDBOL0ZHa0JuZCtzUDFjCkxXbG9tVHB2\nY0NzM0JHbFNkVjVWQkJ1YjdDWk0zdkVBRkoyb1RjUXBEN1R1VFNlNE5PdUVMbkJYZG5HR0lUVUUK\nS044dWNQdGlZcDF1bDZwSGI3U0VWRVdSNVMvdkw4Q2pFcmFqS0ZTQWIySDExTUFmMU1CcEZvZm9v\nUkZJdFNyVQpFNVM2R0dybG15elluRG5OektVNG52b3BlUU1maVNQaHd4M3N2dnZJaEVFU3Z6aVVw\nV2QxcDVRNGlCUXFoZz09Ci0tLS0tRU5EIENFUlRJRklDQVRFLS0tLS0K\n",
+                        "service": {
+                            "name": "beiboot-admission",
+                            "namespace": params.namespace,
+                            "path": "/validate-shelf",
+                        },
+                    },
+                    "failurePolicy": "Fail",
+                    "matchPolicy": "Equivalent",
+                    "name": "validate-shelf.shelf.beiboots.getdeck.dev",
+                    "namespaceSelector": {},
+                    "objectSelector": {},
+                    "rules": [
+                        {
+                            "apiGroups": ["beiboots.getdeck.dev"],
+                            "apiVersions": ["v1"],
+                            "operations": ["CREATE"],
+                            "resources": ["shelves"],
+                            "scope": "*",
+                        }
+                    ],
+                    "sideEffects": "None",
+                    "timeoutSeconds": 30,
+                }
+            ],
+        },
     ]
```

### Comparing `beiboot-1.3.1/beiboot/misc/install.py` & `beiboot-1.4.0/beiboot/misc/install.py`

 * *Files identical despite different names*

### Comparing `beiboot-1.3.1/beiboot/misc/uninstall.py` & `beiboot-1.4.0/beiboot/misc/uninstall.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,23 @@
             name="beiboots.getdeck.dev"
         )
     except k8s.client.exceptions.ApiException as e:  # type: ignore
         if e.status == 404:
             return
         else:
             raise e from None
+    try:
+        config.K8S_EXTENSIONS_API.delete_custom_resource_definition(
+            name="shelves.beiboots.getdeck.dev"
+        )
+    except k8s.client.exceptions.ApiException as e:  # type: ignore
+        if e.status == 404:
+            return
+        else:
+            raise e from None
 
 
 def remove_beiboot_rbac(config: ClientConfiguration):
     try:
         config.K8S_RBAC_API.delete_cluster_role_binding(name="getdeck-beiboot-operator")
     except k8s.client.exceptions.ApiException as e:  # type: ignore
         if e.status == 404:
```

### Comparing `beiboot-1.3.1/beiboot/types.py` & `beiboot-1.4.0/beiboot/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,96 @@
 from datetime import datetime
 from time import sleep
 
 import kubernetes as k8s
 
 from dataclasses import dataclass, field, fields
 from enum import Enum
-from typing import Dict, Optional, Any, Union
+from typing import Dict, Optional, Any, Union, Type
 
 from beiboot.configuration import (
     default_configuration,
     ClientConfiguration,
     __VERSION__,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
+class StateAndEventsMixin:
+    # this mixin is used by Beiboot and Shelf
+    # following class variables need to be set by class that uses this mixin
+    StateClass: Optional[Union[Type["BeibootState"], Type["ShelfState"]]] = None
+    # the uid from Kubernetes for this object
+    uid: str
+    _data: Optional[Dict[str, Any]] = None
+    _config: ClientConfiguration  # check for shelf
+
+    @property
+    def state(self):
+        self.fetch_object()
+        return self.StateClass(self._data.get("state"))
+
+    def fetch_object(self):
+        raise NotImplementedError
+
+    def wait_for_state(
+        self, awaited_state: Union["BeibootState", "ShelfState"], timeout: int = 60
+    ):
+        """
+        > Wait for the state of the resource to be the awaited state, or raise an error if the timeout is reached
+
+        :param awaited_state: The state we're waiting for
+        :type awaited_state: State enum class
+        :param timeout: The maximum time to wait for the state to change, defaults to 60
+        :type timeout: int (optional)
+        :return: the state of the resource.
+        """
+        _i = 0
+        while _i < timeout:
+            if self.state == awaited_state:
+                logger.info(
+                    f"Done waiting for state {awaited_state.value} (is: {self.state.value}, {_i}s/{timeout}s) "
+                )
+                return
+            else:
+                logger.info(
+                    f"Waiting for state {awaited_state.value} (is: {self.state.value}, {_i}s/{timeout}s) "
+                )
+                sleep(1)
+                _i = _i + 1
+        if self.state != awaited_state:
+            raise RuntimeError(f"Waiting for state {awaited_state.value} failed")
+
+    @property
+    def events_by_timestamp(self) -> dict[datetime, Any]:
+        """
+        This function returns a dictionary of events related to this resource, sorted by timestamp
+        :return: A dictionary of events sorted by timestamp.
+        """
+        try:
+            events = self._config.K8S_CORE_API.list_namespaced_event(
+                namespace=self._config.NAMESPACE
+            )
+            related_events = list(
+                filter(lambda et: et.involved_object.uid == self.uid, events.items)
+            )
+        except k8s.client.ApiException as e:  # type: ignore
+            raise RuntimeError(str(e)) from None
+        result = {}
+        for revent in related_events:
+            result[revent.event_time] = {
+                "reason": revent.reason,
+                "reporter": revent.reporting_component,
+                "message": revent.message,
+            }
+        return dict(sorted(result.items()))
+
+
 class BeibootProvider(Enum):
     K3S = "k3s"
 
 
 @dataclass
 class GefyraParams:
     # deploy Gefyra components to this Beiboot
@@ -107,47 +177,51 @@
 class BeibootRequest:
     # a unique name for this Beiboot cluster
     name: str
     # the K8s provider running the cluster
     provider: BeibootProvider = field(default_factory=lambda: BeibootProvider.K3S)
     parameters: BeibootParameters = field(default_factory=lambda: BeibootParameters())
     labels: Dict[str, str] = field(default_factory=lambda: {})
+    from_shelf: str = field(default_factory=lambda: "")
 
 
 class BeibootState(Enum):
     REQUESTED = "REQUESTED"
+    PREPARING = "PREPARING"
+    RESTORING = "RESTORING"
     CREATING = "CREATING"
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     READY = "READY"
     TERMINATING = "TERMINATING"
     ERROR = "ERROR"
 
 
-class Beiboot:
+class Beiboot(StateAndEventsMixin):
     # the final name of this cluster
     name: str
     # the namespace this cluster runs in the host cluster
     namespace: str
-    # the uid from Kubernetes for this object
-    uid: str
     # the beiboot.getdeck.dev object namespace
     object_namespace: str
     # the labels of this Beiboot object
     labels: Dict[str, str]
     # the timestamp when this cluster gets removed
     sunset: Optional[str] = None
     # the timestamp when any client reported its last heartbeat
     last_client_contact: Optional[str] = None
     # all state transitions
     transitions: Optional[dict[str, str]]
     # the cluster parameters
     parameters: BeibootParameters
     provider: str
 
+    # class variables from StateMixin (_data is set in _init_data(...))
+    StateClass = BeibootState
+
     def __init__(
         self, beiboot: dict, config: ClientConfiguration = default_configuration
     ):
         self.name = beiboot["metadata"]["name"]
         self.uid = beiboot["metadata"]["uid"]
         self.labels = beiboot["metadata"].get("labels")
         self.object_namespace = beiboot["metadata"]["namespace"]
@@ -159,19 +233,14 @@
         self._data = _object
         self.namespace = str(self._data.get("beibootNamespace"))
         self.sunset = self._data.get("sunset")
         self.last_client_contact = self._data.get("lastClientContact")
         self.transitions = self._data.get("stateTransitions")
         self.parameters = BeibootParameters.from_raw(self._data["parameters"])
 
-    @property
-    def state(self):
-        self.fetch_object()
-        return BeibootState(self._data.get("state"))
-
     def fetch_object(self):
         logger.debug(f"Fetching object Beiboot {self.name}")
         try:
             bbt = self._config.K8S_CUSTOM_OBJECT_API.get_namespaced_custom_object(
                 group="getdeck.dev",
                 version="v1",
                 namespace=self._config.NAMESPACE,
@@ -193,16 +262,17 @@
         It returns the kubeconfig of the Beiboot.
         :return: The kubeconfig object is being returned.
         """
         from beiboot.utils import decode_kubeconfig
 
         if self.state != BeibootState.READY:
             logger.warning("This Beiboot is not in READY state")
-        kubeconfig_object = self._data.get("kubeconfig")  # noqa
-        if kubeconfig_object is None:
+        if self._data and "kubeconfig" in self._data:
+            kubeconfig_object: Dict[str, str] = self._data["kubeconfig"]  # noqa
+        else:
             return None
         try:
             kubeconfig = decode_kubeconfig(kubeconfig_object)
         except (KeyError, binascii.Error) as e:
             raise RuntimeError(f"Can not fetch kubeconfig: {e}") from None
         else:
             return kubeconfig
@@ -245,68 +315,18 @@
                     raise RuntimeError(
                         f"There was an error decoding the serviceaccount token: {e}"
                     ) from None
         return None
 
     @property
     def tunnel(self) -> Optional[dict[str, Any]]:
-        if tunnel := self._data.get("tunnel"):
-            return tunnel
+        if self._data and "tunnel" in self._data:
+            return self._data["tunnel"]
         return None
 
-    @property
-    def events_by_timestamp(self) -> dict[datetime, Any]:
-        """
-        This function returns a dictionary of events related to this Beiboot, sorted by timestamp
-        :return: A dictionary of events sorted by timestamp.
-        """
-        try:
-            events = self._config.K8S_CORE_API.list_namespaced_event(
-                namespace=self._config.NAMESPACE
-            )
-            related_events = list(
-                filter(lambda et: et.involved_object.uid == self.uid, events.items)
-            )
-        except k8s.client.ApiException as e:  # type: ignore
-            raise RuntimeError(str(e)) from None
-        result = {}
-        for revent in related_events:
-            result[revent.event_time] = {
-                "reason": revent.reason,
-                "reporter": revent.reporting_component,
-                "message": revent.message,
-            }
-        return dict(sorted(result.items()))
-
-    def wait_for_state(self, awaited_state: BeibootState, timeout: int = 60):
-        """
-        > Wait for the state of the Beiboot to be the awaited state, or raise an error if the timeout is reached
-
-        :param awaited_state: The state we're waiting for
-        :type awaited_state: BeibootState
-        :param timeout: The maximum time to wait for the state to change, defaults to 60
-        :type timeout: int (optional)
-        :return: the state of the beiboot.
-        """
-        _i = 0
-        while _i < timeout:
-            if self.state == awaited_state:
-                logger.info(
-                    f"Done waiting for state {awaited_state.value} (is: {self.state.value}, {_i}s/{timeout}s) "
-                )
-                return
-            else:
-                logger.info(
-                    f"Waiting for state {awaited_state.value} (is: {self.state.value}, {_i}s/{timeout}s) "
-                )
-                sleep(1)
-                _i = _i + 1
-        if self.state != awaited_state:
-            raise RuntimeError(f"Waiting for state {awaited_state.value} failed")
-
 
 @dataclass
 class InstallOptions:
     namespace: str = field(
         default_factory=lambda: "getdeck",
         metadata=dict(
             help="The namespace to install Beiboot into (default: getdeck)", short="ns"
@@ -317,21 +337,21 @@
         metadata=dict(
             help="Set the Operator version; components are created according to this beibootctl version"
         ),
     )
     storage_class: str = field(
         default_factory=lambda: "standard",
         metadata=dict(
-            help="Set the Kubernetes storageClassName of PVCs created for Beiboot clusters (default: standard)"
+            help="Set the Kubernetes StorageClass of PVCs created for Beiboot clusters (default: standard)"
         ),
     )
     shelf_storage_class: str = field(
         default_factory=lambda: "standard",
         metadata=dict(
-            help="Set the Kubernetes storageClassName of VolumeSnapshots created for Beiboot shelf clusters (default: standard)"
+            help="Set the Kubernetes VolumeSnapshotClass of VolumeSnapshots created for Beiboot shelf clusters (default: standard)"  # noqa: E501
         ),
     )
     node_storage_request: str = field(
         default_factory=lambda: "1Gi",
         metadata=dict(
             help="The default storage request for Beiboot nodes (default: 1Gi)"
         ),
@@ -384,7 +404,94 @@
     )
     node_requests_memory: str = field(
         default_factory=lambda: "1Gi",
         metadata=dict(
             help="The default memory request for each Beiboot node pod (default: 1Gi)",
         ),
     )
+
+
+@dataclass
+class VolumeSnapshotContentStatus(Enum):
+    NOT_READY_TO_USE = "NOT_READY_TO_USE"
+    READY_TO_USE = "READY_TO_USE"
+
+
+@dataclass
+class VolumeSnapshotContent:
+    name: str
+    snapshot_handle: str
+    node: str
+    status: VolumeSnapshotContentStatus = field(
+        default_factory=lambda: VolumeSnapshotContentStatus.NOT_READY_TO_USE
+    )
+
+
+@dataclass
+class ShelfRequest:
+    # a unique name for this Shelf
+    name: str
+    cluster_name: str
+    volume_snapshot_class: str = ""
+    volume_snapshot_contents: list[VolumeSnapshotContent] = field(
+        default_factory=lambda: []
+    )
+    labels: Dict[str, str] = field(default_factory=lambda: {})
+
+
+class ShelfState(Enum):
+    REQUESTED = "REQUESTED"
+    CREATING = "CREATING"
+    PREPARING = "PREPARING"
+    PENDING = "PENDING"
+    READY = "READY"
+    TERMINATING = "TERMINATING"
+    ERROR = "ERROR"
+
+
+class Shelf(StateAndEventsMixin):
+    # the final name of this cluster
+    name: str
+    # the namespace this shelf is located in the host cluster (currently it's always "getdeck")
+    namespace: str
+    # list of VolumeSnapshotContents that are contained in this shelf
+    volume_snapshot_contents: Optional[list[VolumeSnapshotContent]]
+    # the labels of this Beiboot object
+    labels: Dict[str, str]
+    # all state transitions
+    transitions: Optional[dict[str, str]]
+
+    # class variables from StateMixin (_data is set in _init_data(...))
+    StateClass = ShelfState
+
+    def __init__(
+        self, shelf: dict, config: ClientConfiguration = default_configuration
+    ):
+        self.name = shelf["metadata"]["name"]
+        self.uid = shelf["metadata"]["uid"]
+        self.labels = shelf["metadata"].get("labels")
+        self._init_data(shelf)
+        self._config = config
+
+    def _init_data(self, _object: dict[str, Any]):
+        self._data = _object
+        self.transitions = self._data.get("stateTransitions")
+        self.volume_snapshot_contents = self._data.get("volumeSnapshotContents")
+
+    def fetch_object(self):
+        logger.debug(f"Fetching object Shelf {self.name}")
+        try:
+            shelf = self._config.K8S_CUSTOM_OBJECT_API.get_namespaced_custom_object(
+                group="beiboots.getdeck.dev",
+                version="v1",
+                namespace=self._config.NAMESPACE,
+                plural="shelves",
+                name=self.name,
+            )
+        except k8s.client.exceptions.ApiException as e:  # type: ignore
+            if e.status == 404:
+                raise RuntimeError(
+                    f"The Shelf '{self.name}' does not exist anymore"
+                ) from None
+            else:
+                raise RuntimeError(str(e)) from None
+        self._init_data(shelf)  # type: ignore
```

### Comparing `beiboot-1.3.1/beiboot/utils.py` & `beiboot-1.4.0/beiboot/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,29 +2,50 @@
 import logging
 import socket
 from pathlib import Path
 from typing import List, Optional, Container
 
 from beiboot.configuration import ClientConfiguration, __VERSION__
 
-from beiboot.types import BeibootRequest
+from beiboot.types import BeibootRequest, ShelfRequest
 
 logger = logging.getLogger(__name__)
 
 
 def create_beiboot_custom_ressource(
     req: BeibootRequest, config: ClientConfiguration
 ) -> dict:
     _labels = req.labels
     _labels.update({"beiboot.getdeck.dev/client-version": __VERSION__})
     cr = {
         "apiVersion": "getdeck.dev/v1",
         "kind": "beiboot",
         "provider": "k3s",
         "parameters": req.parameters.as_dict(),
+        "fromShelf": req.from_shelf,
+        "metadata": {
+            "name": req.name,
+            "namespace": config.NAMESPACE,
+            "labels": _labels,
+        },
+    }
+    return cr
+
+
+def create_shelf_custom_ressource(
+    req: ShelfRequest, config: ClientConfiguration
+) -> dict:
+    _labels = req.labels
+    _labels.update({"beiboot.getdeck.dev/client-version": __VERSION__})
+    cr = {
+        "apiVersion": "beiboots.getdeck.dev/v1",
+        "kind": "shelf",
+        "clusterName": req.cluster_name,
+        "volumeSnapshotClass": req.volume_snapshot_class,
+        "volumeSnapshotContents": req.volume_snapshot_contents,
         "metadata": {
             "name": req.name,
             "namespace": config.NAMESPACE,
             "labels": _labels,
         },
     }
     return cr
```

### Comparing `beiboot-1.3.1/PKG-INFO` & `beiboot-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beiboot
-Version: 1.3.1
+Version: 1.4.0
 Summary: Getdeck Beiboot client project.
 Home-page: https://getdeck.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@blueshoe.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

