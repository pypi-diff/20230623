# Comparing `tmp/mse_cli_core-0.1a6.tar.gz` & `tmp/mse_cli_core-0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a6.tar", last modified: Thu Jun 22 08:32:31 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a7.tar", last modified: Fri Jun 23 07:12:22 2023, max compression
```

## Comparing `mse_cli_core-0.1a6.tar` & `mse_cli_core-0.1a7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.286998 mse_cli_core-0.1a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.286998 mse_cli_core-0.1a6/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.305821 mse_cli_core-0.1a7/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-23 07:12:22.305821 mse_cli_core-0.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-23 07:12:22.305821 mse_cli_core-0.1a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.293821 mse_cli_core-0.1a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.301821 mse_cli_core-0.1a7/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.301821 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.301821 mse_cli_core-0.1a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a6/PKG-INFO` & `mse_cli_core-0.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli_core
-Version: 0.1a6
+Version: 0.1a7
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a6/setup.cfg` & `mse_cli_core-0.1a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/setup.py` & `mse_cli_core-0.1a7/setup.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a7/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a7/src/mse_cli_core/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a7/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a7/src/mse_cli_core/enclave.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """mse_cli_core.enclave module."""
 
 import re
+import uuid
 from pathlib import Path
 from typing import Optional, Tuple, Union
 
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.x509 import Certificate, CertificateRevocationList
 from docker.client import DockerClient
+from docker.errors import NotFound
 from intel_sgx_ra.attest import verify_quote
 from intel_sgx_ra.ratls import ratls_verify
 from intel_sgx_ra.signer import mr_signer_from_pk
 
 from mse_cli_core.no_sgx_docker import NoSgxDockerConfig
 
 
@@ -26,31 +28,50 @@
     client: DockerClient,
     image: str,
     app_args: NoSgxDockerConfig,
     app_path: Path,
     docker_path_log: Path,
 ) -> str:
     """Compute the MR enclave."""
-    container = client.containers.run(
-        image,
-        command=app_args.cmd(),
-        volumes=app_args.volumes(app_path),
-        entrypoint=NoSgxDockerConfig.entrypoint,
-        remove=True,
-        detach=False,
-        stdout=True,
-        stderr=True,
-    )
+    container_name = str(uuid.uuid4())
+    output = b""
 
-    # Save the docker output
-    docker_path_log.write_bytes(container)
+    try:
+        container = client.containers.run(
+            image,
+            name=container_name,
+            command=app_args.cmd(),
+            volumes=app_args.volumes(app_path),
+            entrypoint=NoSgxDockerConfig.entrypoint,
+            # We do not remove the container to be able to print the error (if some)
+            remove=False,
+            detach=False,
+            stdout=True,
+            stderr=True,
+        )
+    except Exception as exc:
+        raise Exception(
+            f"Error starting the docker (see logs at {docker_path_log})"
+        ) from exc
+    finally:
+        try:
+            container = client.containers.get(container_name)
+            # Save the docker output
+            output = container.logs()
+            docker_path_log.write_bytes(output)
+            container.stop(timeout=1)
+            # We need to remove the container since we declare remove=False previously
+            container.remove()
+
+        except NotFound:
+            pass
 
     # Get the mr_enclave from the docker output
     pattern = "Measurement:\n[ ]*([a-z0-9]{64})"
-    m = re.search(pattern.encode("utf-8"), container)
+    m = re.search(pattern.encode("utf-8"), output)
 
     if not m:
         raise Exception(
             f"Fail to compute mr_enclave! See {docker_path_log} for more details."
         )
 
     return str(m.group(1).decode("utf-8"))
```

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a7/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a7/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a7/src/mse_cli_core/no_sgx_docker.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class NoSgxDockerConfig(BaseModel):
     """Definition of an mse docker running on a non-sgx hardware."""
 
     host: str
     expiration_date: Optional[int]
-    app_cert: Optional[Path]
     size: int
     app_id: UUID
     application: str
 
     app_mountpoint: ClassVar[str] = "/opt/input"
     entrypoint: ClassVar[str] = "mse-run"
 
@@ -32,15 +31,15 @@
             "--id",
             str(self.app_id),
             "--application",
             self.application,
             "--dry-run",
         ]
 
-        if not self.app_cert:
+        if self.expiration_date:
             command.append("--expiration")
             command.append(str(self.expiration_date))
 
         return command
 
     def volumes(self, app_path: Path) -> Dict[str, Dict[str, str]]:
         """Define the docker volumes."""
```

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a7/src/mse_cli_core/sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/spinner.py` & `mse_cli_core-0.1a7/src/mse_cli_core/spinner.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a7/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a7/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli-core
-Version: 0.1a6
+Version: 0.1a7
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a6/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a7/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/tests/test_base64.py` & `mse_cli_core-0.1a7/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/tests/test_boostrap.py` & `mse_cli_core-0.1a7/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/tests/test_ignore_file.py` & `mse_cli_core-0.1a7/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/tests/test_no_sgx_docker.py` & `mse_cli_core-0.1a7/tests/test_no_sgx_docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,29 +46,14 @@
     assert ref_conf.volumes(Path("/tmp/")) == {
         "/tmp": {
             "bind": "/opt/input",
             "mode": "rw",
         }
     }
 
-    ref_conf = NoSgxDockerConfig(
-        host="localhost",
-        app_cert="/app/cert.pem",
-        size=4096,
-        app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
-        application="app:app",
-    )
-
-    assert ref_conf.volumes(Path("/tmp/")) == {
-        "/tmp": {
-            "bind": "/opt/input",
-            "mode": "rw",
-        }
-    }
-
 
 def test_cmd():
     """Test `cmd` function."""
     ref_conf = NoSgxDockerConfig(
         host="localhost",
         expiration_date=1714058115,
         size=4096,
@@ -88,15 +73,14 @@
         "--dry-run",
         "--expiration",
         "1714058115",
     ]
 
     ref_conf = NoSgxDockerConfig(
         host="localhost",
-        app_cert="cert.pem",
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     assert ref_conf.cmd() == [
         "--size",
```

### Comparing `mse_cli_core-0.1a6/tests/test_sgx_docker.py` & `mse_cli_core-0.1a7/tests/test_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a6/tests/test_test_docker.py` & `mse_cli_core-0.1a7/tests/test_test_docker.py`

 * *Files identical despite different names*

