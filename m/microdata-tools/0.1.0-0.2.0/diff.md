# Comparing `tmp/microdata_tools-0.1.0.tar.gz` & `tmp/microdata_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_tools-0.1.0.tar", max compression
+gzip compressed data, was "microdata_tools-0.2.0.tar", max compression
```

## Comparing `microdata_tools-0.1.0.tar` & `microdata_tools-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     2203 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/README.md
--rw-r--r--   0        0        0      176 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/__init__.py
--rw-r--r--   0        0        0     4008 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/_decrypt.py
--rw-r--r--   0        0        0     4235 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/_encrypt.py
--rw-r--r--   0        0        0      212 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/_utils.py
--rw-r--r--   0        0        0      141 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/exceptions.py
--rw-r--r--   0        0        0     1331 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/package_dataset.py
--rw-r--r--   0        0        0     2341 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/unpackage_dataset.py
--rw-r--r--   0        0        0      534 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 microdata_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2232 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/README.md
+-rw-r--r--   0        0        0      176 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/__init__.py
+-rw-r--r--   0        0        0     5722 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/_decrypt.py
+-rw-r--r--   0        0        0     4562 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/_encrypt.py
+-rw-r--r--   0        0        0      212 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/_utils.py
+-rw-r--r--   0        0        0      141 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/exceptions.py
+-rw-r--r--   0        0        0     1904 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/package_dataset.py
+-rw-r--r--   0        0        0     2341 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/microdata_tools/unpackage_dataset.py
+-rw-r--r--   0        0        0      534 2023-06-23 13:29:09.501447 microdata_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 microdata_tools-0.2.0/PKG-INFO
```

### Comparing `microdata_tools-0.1.0/LICENSE.md` & `microdata_tools-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.1.0/README.md` & `microdata_tools-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # microdata-tools
-Tools for the microdata.no platform
+Tools for the [microdata.no](https://www.microdata.no/) platform
 
 ## Installation
 `microdata-tools` can be installed from PyPI using pip:
 ```
 pip install microdata-tools
 ```
```

### Comparing `microdata_tools-0.1.0/microdata_tools/_encrypt.py` & `microdata_tools-0.2.0/microdata_tools/_encrypt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import logging
 import os
 from pathlib import Path
-import shutil
 import tarfile
+import shutil
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 
 from microdata_tools.exceptions import ValidationException
 from microdata_tools._utils import check_exists
 
 logger = logging.getLogger()
 
+CHUNK_SIZE_BYTES = 250_000_000  # 250 MB per chunk
 
-def _encrypt_dataset(rsa_keys_dir: Path, dataset_dir: Path, output_dir: Path) -> None:
+
+def encrypt_dataset(
+    rsa_keys_dir: Path,
+    dataset_dir: Path,
+    output_dir: Path,
+) -> None:
     """
     Encrypts a dataset as follows:
         1. Generates the symmetric key for this dataset.
-        2. Encrypts the dataset using the symmetric key.
-        3. Encrypts the symmetric key using the RSA public key.
+        2. Splits the dataset into chunks.
+        3. Encrypts each chunk using the symmetric key.
+        4. Encrypts the symmetric key using the RSA public key.
     """
 
     check_exists(rsa_keys_dir)
     check_exists(dataset_dir)
 
     if not output_dir.exists():
         os.makedirs(output_dir)
@@ -37,49 +44,51 @@
     with open(public_key_location, "rb") as key_file:
         public_key = serialization.load_pem_public_key(
             key_file.read(), backend=default_backend()
         )
 
     csv_files = [file for file in dataset_dir.iterdir() if file.suffix == ".csv"]
 
-    if len(csv_files) == 0:
-        raise ValidationException(f"No csv files found in {dataset_dir}")
-
-    if len(csv_files) > 1:
-        raise ValidationException(f"There should only be one csv file in {dataset_dir}")
-
     csv_file = csv_files[0]
     dataset_name = csv_file.stem
 
     if dataset_name != dataset_dir.stem:
         raise ValidationException(
             f"The csv file name {dataset_name} should match "
             f"the dataset directory name {dataset_dir.stem}."
         )
 
     dataset_output_dir = output_dir / dataset_name
     os.makedirs(dataset_output_dir)
+    os.makedirs(dataset_output_dir / "chunks", exist_ok=True)
 
-    encrypted_file = dataset_output_dir / f"{dataset_name}.csv.encr"
     encrypted_symkey_file = dataset_output_dir / f"{dataset_name}.symkey.encr"
 
     # Generate and store symmetric key for this file
     symkey = Fernet.generate_key()
+    fernet = Fernet(symkey)
 
     # Encrypt csv file
-    with open(csv_file, "rb") as file:
-        data = file.read()  # Read the bytes of the input file
+    chunk_count = 0
+    logger.debug(f"Chunk size: {CHUNK_SIZE_BYTES} Bytes")
 
-    fernet = Fernet(symkey)
-    encrypted = fernet.encrypt(data)
-
-    with open(encrypted_file, "wb") as file:
-        file.write(encrypted)
+    with open(csv_file, "rb") as file:
+        while True:
+            data = file.read(CHUNK_SIZE_BYTES)
+            if not data:
+                break
+
+            chunk_count += 1
+            encrypted = fernet.encrypt(data)
+
+            chunk_file = dataset_output_dir / "chunks" / f"{chunk_count}.csv.encr"
+            with open(chunk_file, "wb") as chunk_output:
+                chunk_output.write(encrypted)
 
-    logger.debug(f"Csv file {csv_file} encrypted into {encrypted_file}")
+    logger.debug(f"Csv file {csv_file} encrypted into {chunk_count} chunks")
 
     encrypted_sym_key = public_key.encrypt(
         symkey,
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None,
@@ -99,30 +108,38 @@
     Removes the input directory after successful completion.
     :param input_dir: the input directory containing the dataset directory
     :param dataset_name: the name of the dataset
     """
 
     check_exists(input_dir)
 
-    if len(list((input_dir / dataset_name).iterdir())) == 0:
-        raise ValidationException(f"No files found in {input_dir / dataset_name}")
+    dataset_dir = input_dir / dataset_name
+
+    if not dataset_dir.exists():
+        raise ValidationException(f"Dataset directory {dataset_dir} not found")
 
     tar_file_name = f"{dataset_name}.tar"
     full_tar_file_name = input_dir / tar_file_name
-    files_to_tar = [
-        input_dir / dataset_name / f"{dataset_name}.csv.encr",
-        input_dir / dataset_name / f"{dataset_name}.symkey.encr",
-        input_dir / dataset_name / f"{dataset_name}.json",
-    ]
 
-    json_file = input_dir / dataset_name / f"{dataset_name}.json"
+    json_file = dataset_dir / f"{dataset_name}.json"
     if not json_file.exists():
         raise ValidationException(f"The required file {json_file} not found")
 
+    files_to_tar = [dataset_dir / f"{dataset_name}.json"]
+    chunk_dir = dataset_dir / "chunks"
+
+    if chunk_dir.exists():
+        chunk_files = [file for file in chunk_dir.iterdir()]
+        if len(chunk_files) == 0:
+            raise ValidationException(f"No files found in {chunk_dir}")
+
+        files_to_tar.extend([dataset_dir / f"{dataset_name}.symkey.encr"])
+
     with tarfile.open(full_tar_file_name, "w") as tar:
         for file in files_to_tar:
-            if file.exists():
-                logger.debug(f"Adding {file} to tar..")
-                tar.add(file, arcname=file.name)
+            tar.add(file, arcname=os.path.basename(file))
+        if chunk_dir.exists():
+            tar.add(chunk_dir, arcname=os.path.basename(chunk_dir))
+
+    shutil.rmtree(dataset_dir)
 
-    shutil.rmtree(input_dir / dataset_name)
     logger.debug(f"Archive {full_tar_file_name} created")
```

### Comparing `microdata_tools-0.1.0/microdata_tools/unpackage_dataset.py` & `microdata_tools-0.2.0/microdata_tools/unpackage_dataset.py`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.1.0/pyproject.toml` & `microdata_tools-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microdata-tools"
-version = "0.1.0"
+version = "0.2.0"
 description = "Tools for the microdata.no platform"
 authors = ["microdata-developers"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "microdata_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `microdata_tools-0.1.0/PKG-INFO` & `microdata_tools-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: microdata-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tools for the microdata.no platform
 License: MIT
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Description-Content-Type: text/markdown
 
 # microdata-tools
-Tools for the microdata.no platform
+Tools for the [microdata.no](https://www.microdata.no/) platform
 
 ## Installation
 `microdata-tools` can be installed from PyPI using pip:
 ```
 pip install microdata-tools
 ```
```

