# Comparing `tmp/nucypher_core-0.8.0.tar.gz` & `tmp/nucypher_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucypher_core-0.8.0.tar", last modified: Tue May 23 18:41:53 2023, max compression
+gzip compressed data, was "nucypher_core-0.9.0.tar", last modified: Wed Jun  7 11:41:54 2023, max compression
```

## Comparing `nucypher_core-0.8.0.tar` & `nucypher_core-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 18:41:52.000000 nucypher_core-0.8.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/nucypher_core/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/umbral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/umbral.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/nucypher_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:41:54.363203 nucypher_core-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-07 11:41:54.000000 nucypher_core-0.9.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 11:41:54.363203 nucypher_core-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:41:54.359203 nucypher_core-0.9.0/nucypher_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/ferveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/ferveo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/umbral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/nucypher_core/umbral.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:41:54.359203 nucypher_core-0.9.0/nucypher_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 11:41:54.000000 nucypher_core-0.9.0/nucypher_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 11:41:54.000000 nucypher_core-0.9.0/nucypher_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:41:54.000000 nucypher_core-0.9.0/nucypher_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:41:54.000000 nucypher_core-0.9.0/nucypher_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 11:41:54.000000 nucypher_core-0.9.0/nucypher_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:41:54.363203 nucypher_core-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:41:54.359203 nucypher_core-0.9.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    39154 2023-06-07 11:41:50.000000 nucypher_core-0.9.0/src/lib.rs
```

### Comparing `nucypher_core-0.8.0/LICENSE` & `nucypher_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.8.0/PKG-INFO` & `nucypher_core-0.9.0/nucypher_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nucypher_core
-Version: 0.8.0
+Name: nucypher-core
+Version: 0.9.0
 Summary: Protocol structures of Nucypher network
 Home-page: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nucypher_core-0.8.0/README.md` & `nucypher_core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.8.0/nucypher_core/__init__.pyi` & `nucypher_core-0.9.0/nucypher_core/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,19 @@
     Signer,
     Capsule,
     VerifiedKeyFrag,
     VerifiedCapsuleFrag,
     RecoverableSignature
 )
 
+from .ferveo import  (
+    FerveoPublicKey,
+    Ciphertext
+)
+
 
 class Address:
 
     def __init__(self, address_bytes: bytes):
         ...
 
     def __bytes__(self) -> bytes:
@@ -296,29 +301,29 @@
     def __init__(
         self,
         staking_provider_address: Address,
         domain: str,
         timestamp_epoch: int,
         verifying_key: PublicKey,
         encrypting_key: PublicKey,
-        ferveo_public_key: bytes,
+        ferveo_public_key: FerveoPublicKey,
         certificate_der: bytes,
         host: str,
         port: int,
         operator_signature: RecoverableSignature,
     ):
         ...
 
     staking_provider_address: Address
 
     verifying_key: PublicKey
 
     encrypting_key: PublicKey
 
-    ferveo_public_key: bytes
+    ferveo_public_key: FerveoPublicKey
 
     operator_signature: RecoverableSignature
 
     domain: str
 
     host: str
 
@@ -401,94 +406,131 @@
 
     def __bytes__(self) -> bytes:
         ...
 
 
 class ThresholdDecryptionRequest:
 
-    def __init__(self, ritual_id: int, variant: int, ciphertext: bytes, conditions: Optional[Conditions], context: Optional[Context]):
+    def __init__(self, ritual_id: int, variant: int, ciphertext: Ciphertext, conditions: Optional[Conditions], context: Optional[Context]):
         ...
 
     ritual_id: int
 
     conditions: Optional[Conditions]
 
     context: Optional[Context]
 
     variant: int
 
-    ciphertext: bytes
+    ciphertext: Ciphertext
 
-    def encrypt(self, request_encrypting_key: PublicKey, response_encrypting_key: PublicKey) -> EncryptedThresholdDecryptionRequest:
+    def encrypt(self, shared_secret: SessionSharedSecret, requester_public_key: SessionStaticKey) -> EncryptedThresholdDecryptionRequest:
         ...
 
     @staticmethod
     def from_bytes(data: bytes) -> ThresholdDecryptionRequest:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
-class E2EThresholdDecryptionRequest:
-
-    decryption_request: ThresholdDecryptionRequest
-
-    response_encrypting_key: PublicKey
-
-    @staticmethod
-    def from_bytes(data: bytes) -> E2EThresholdDecryptionRequest:
-        ...
-
-    def __bytes__(self) -> bytes:
-        ...
-
-
 class EncryptedThresholdDecryptionRequest:
     ritual_id: int
 
+    requester_public_key: SessionStaticKey
+
     def decrypt(
         self,
-        sk: SecretKey
-    ) -> E2EThresholdDecryptionRequest:
+        shared_secret: SessionSharedSecret
+    ) -> ThresholdDecryptionRequest:
         ...
 
     @staticmethod
     def from_bytes(data: bytes) -> EncryptedThresholdDecryptionRequest:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
 class ThresholdDecryptionResponse:
 
-    def __init__(self, decryption_share: bytes):
+    def __init__(self, ritual_id: int, decryption_share: bytes):
         ...
 
     decryption_share: bytes
 
-    def encrypt(self, encrypting_key: PublicKey) -> EncryptedThresholdDecryptionResponse:
+    ritual_id: int
+
+    def encrypt(self, shared_secret: SessionSharedSecret) -> EncryptedThresholdDecryptionResponse:
         ...
 
     @staticmethod
     def from_bytes(data: bytes) -> ThresholdDecryptionResponse:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
 class EncryptedThresholdDecryptionResponse:
 
+    ritual_id: int
+
     def decrypt(
         self,
-        sk: SecretKey
+        shared_secret: SessionSharedSecret
     ) -> ThresholdDecryptionResponse:
         ...
 
     @staticmethod
     def from_bytes(data: bytes) -> EncryptedThresholdDecryptionResponse:
         ...
 
     def __bytes__(self) -> bytes:
         ...
+
+
+class SessionSharedSecret:
+    ...
+
+
+class SessionStaticKey:
+
+    @staticmethod
+    def from_bytes(data: bytes) -> SessionStaticKey:
+        ...
+
+    def __bytes__(self) -> bytes:
+        ...
+
+
+class SessionStaticSecret:
+
+    @staticmethod
+    def random() -> SessionStaticSecret:
+        ...
+
+    def public_key(self) -> SessionStaticKey:
+        ...
+
+    def derive_shared_secret(self, their_public_key: SessionStaticKey) -> SessionSharedSecret:
+        ...
+
+
+class SessionSecretFactory:
+
+    @staticmethod
+    def random() -> SessionSecretFactory:
+        ...
+
+    @staticmethod
+    def seed_size() -> int:
+        ...
+
+    @staticmethod
+    def from_secure_randomness(seed: bytes) -> SessionSecretFactory:
+        ...
+
+    def make_key(self, label: bytes) -> SessionStaticSecret:
+        ...
```

### Comparing `nucypher_core-0.8.0/nucypher_core/umbral.py` & `nucypher_core-0.9.0/nucypher_core/umbral.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ._nucypher_core import umbral as _umbral
 
 SecretKey = _umbral.SecretKey
 PublicKey = _umbral.PublicKey
-SecretKeyFactory =_umbral.SecretKeyFactory
+SecretKeyFactory = _umbral.SecretKeyFactory
 Signature = _umbral.Signature
 RecoverableSignature = _umbral.RecoverableSignature
 Signer = _umbral.Signer
 Capsule = _umbral.Capsule
 KeyFrag = _umbral.KeyFrag
 VerifiedKeyFrag = _umbral.VerifiedKeyFrag
 CapsuleFrag = _umbral.CapsuleFrag
```

### Comparing `nucypher_core-0.8.0/nucypher_core/umbral.pyi` & `nucypher_core-0.9.0/nucypher_core/umbral.pyi`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.8.0/nucypher_core.egg-info/PKG-INFO` & `nucypher_core-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nucypher-core
-Version: 0.8.0
+Name: nucypher_core
+Version: 0.9.0
 Summary: Protocol structures of Nucypher network
 Home-page: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nucypher_core-0.8.0/setup.py` & `nucypher_core-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="nucypher_core",
     description="Protocol structures of Nucypher network",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.8.0",
+    version="0.9.0",
     author="Bogdan Opanchuk",
     author_email="bogdan@opanchuk.net",
     url="https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python",
     rust_extensions=[RustExtension("nucypher_core._nucypher_core", binding=Binding.PyO3, debug=False)],
     packages=["nucypher_core"],
     package_data = {
-        'nucypher_core': ['py.typed', '__init__.pyi', 'umbral.pyi'],
+        'nucypher_core': ['py.typed', '__init__.pyi', 'umbral.pyi', 'ferveo.pyi'],
     },
     # rust extensions are not zip safe, just like C-extensions.
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `nucypher_core-0.8.0/src/lib.rs` & `nucypher_core-0.9.0/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 // Will probably be fixed by Rust 1.65
 #![allow(clippy::borrow_deref_ref)]
 
 extern crate alloc;
 
 use alloc::collections::{BTreeMap, BTreeSet};
 
+use ferveo::bindings_python::{Ciphertext, FerveoPublicKey};
 use pyo3::class::basic::CompareOp;
 use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::pyclass::PyClass;
 use pyo3::types::{PyBytes, PyUnicode};
 use umbral_pre::bindings_python::{
     Capsule, PublicKey, RecoverableSignature, SecretKey, Signer, VerificationError,
@@ -628,30 +629,140 @@
 
     fn __bytes__(&self) -> PyObject {
         to_bytes(self)
     }
 }
 
 //
+// Session Keys
+//
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct SessionSharedSecret {
+    backend: nucypher_core::SessionSharedSecret,
+}
+
+#[pyclass(module = "nucypher_core")]
+#[derive(Clone, PartialEq, Eq, derive_more::From, derive_more::AsRef)]
+pub struct SessionStaticKey {
+    backend: nucypher_core::SessionStaticKey,
+}
+
+#[pymethods]
+impl SessionStaticKey {
+    #[staticmethod]
+    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
+        from_bytes::<_, nucypher_core::SessionStaticKey>(data)
+    }
+
+    fn __bytes__(&self) -> PyObject {
+        to_bytes(self)
+    }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
+        richcmp(self, other, op)
+    }
+
+    fn __hash__(&self) -> PyResult<isize> {
+        hash("SessionStaticKey", self)
+    }
+
+    fn __str__(&self) -> PyResult<String> {
+        Ok(format!("{}", self.backend))
+    }
+}
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct SessionStaticSecret {
+    backend: nucypher_core::SessionStaticSecret,
+}
+
+#[pymethods]
+impl SessionStaticSecret {
+    #[staticmethod]
+    pub fn random() -> PyResult<Self> {
+        Ok(Self {
+            backend: nucypher_core::SessionStaticSecret::random(),
+        })
+    }
+
+    pub fn public_key(&self) -> SessionStaticKey {
+        SessionStaticKey {
+            backend: self.backend.public_key(),
+        }
+    }
+
+    pub fn derive_shared_secret(&self, their_public_key: &SessionStaticKey) -> SessionSharedSecret {
+        SessionSharedSecret {
+            backend: self.backend.derive_shared_secret(their_public_key.as_ref()),
+        }
+    }
+
+    fn __str__(&self) -> String {
+        self.backend.to_string()
+    }
+}
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct SessionSecretFactory {
+    backend: nucypher_core::SessionSecretFactory,
+}
+
+#[pymethods]
+impl SessionSecretFactory {
+    #[staticmethod]
+    pub fn random() -> PyResult<Self> {
+        Ok(Self {
+            backend: nucypher_core::SessionSecretFactory::random(),
+        })
+    }
+
+    #[staticmethod]
+    pub fn seed_size() -> usize {
+        nucypher_core::SessionSecretFactory::seed_size()
+    }
+
+    #[staticmethod]
+    pub fn from_secure_randomness(seed: &[u8]) -> PyResult<Self> {
+        let factory = nucypher_core::SessionSecretFactory::from_secure_randomness(seed)
+            .map_err(|err| PyValueError::new_err(format!("{}", err)))?;
+        Ok(Self { backend: factory })
+    }
+
+    pub fn make_key(&self, label: &[u8]) -> SessionStaticSecret {
+        SessionStaticSecret {
+            backend: self.backend.make_key(label),
+        }
+    }
+
+    fn __str__(&self) -> String {
+        self.backend.to_string()
+    }
+}
+
+//
 // Threshold Decryption Request
 //
 
 #[pyclass(module = "nucypher_core")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct ThresholdDecryptionRequest {
     backend: nucypher_core::ThresholdDecryptionRequest,
 }
 
 #[pymethods]
 impl ThresholdDecryptionRequest {
     #[new]
     pub fn new(
-        ritual_id: u16,
+        ritual_id: u32,
         variant: u8,
-        ciphertext: &[u8], // TODO use ferveo Ciphertext type
+        ciphertext: &Ciphertext,
         conditions: Option<&Conditions>,
         context: Option<&Context>,
     ) -> PyResult<Self> {
         let ferveo_variant = match variant {
             0 => FerveoVariant::SIMPLE,
             1 => FerveoVariant::PRECOMPUTED,
             _ => {
@@ -660,26 +771,26 @@
                 ))
             }
         };
 
         Ok(Self {
             backend: nucypher_core::ThresholdDecryptionRequest::new(
                 ritual_id,
-                ciphertext,
+                ciphertext.as_ref(),
                 conditions
                     .map(|conditions| conditions.backend.clone())
                     .as_ref(),
                 context.map(|context| context.backend.clone()).as_ref(),
                 ferveo_variant,
             ),
         })
     }
 
     #[getter]
-    pub fn ritual_id(&self) -> u16 {
+    pub fn ritual_id(&self) -> u32 {
         self.backend.ritual_id
     }
 
     #[getter]
     pub fn conditions(&self) -> Option<Conditions> {
         self.backend
             .conditions
@@ -694,101 +805,78 @@
         self.backend
             .context
             .clone()
             .map(|context| Context { backend: context })
     }
 
     #[getter]
-    pub fn ciphertext(&self) -> &[u8] {
-        self.backend.ciphertext.as_ref()
+    pub fn ciphertext(&self) -> Ciphertext {
+        self.backend.ciphertext.clone().into()
     }
 
     #[getter]
     pub fn variant(&self) -> u8 {
         match self.backend.variant {
             FerveoVariant::SIMPLE => 0,
             FerveoVariant::PRECOMPUTED => 1,
         }
     }
 
     pub fn encrypt(
         &self,
-        request_encrypting_key: &PublicKey,
-        response_encrypting_key: &PublicKey,
+        shared_secret: &SessionSharedSecret,
+        requester_public_key: &SessionStaticKey,
     ) -> EncryptedThresholdDecryptionRequest {
+        let encrypted_request = self
+            .backend
+            .encrypt(shared_secret.as_ref(), requester_public_key.as_ref());
         EncryptedThresholdDecryptionRequest {
-            backend: self.backend.encrypt(
-                request_encrypting_key.as_ref(),
-                response_encrypting_key.as_ref(),
-            ),
+            backend: encrypted_request,
         }
     }
 
     #[staticmethod]
     pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
         from_bytes::<_, nucypher_core::ThresholdDecryptionRequest>(data)
     }
 
     fn __bytes__(&self) -> PyObject {
         to_bytes(self)
     }
 }
 
 //
-// E2EThresholdDecryptionRequest
-//
-#[pyclass(module = "nucypher_core")]
-#[derive(derive_more::From, derive_more::AsRef)]
-pub struct E2EThresholdDecryptionRequest {
-    backend: nucypher_core::E2EThresholdDecryptionRequest,
-}
-
-#[pymethods]
-impl E2EThresholdDecryptionRequest {
-    #[getter]
-    pub fn decryption_request(&self) -> ThresholdDecryptionRequest {
-        self.backend.decryption_request.clone().into()
-    }
-
-    #[getter]
-    pub fn response_encrypting_key(&self) -> PublicKey {
-        self.backend.response_encrypting_key.into()
-    }
-
-    #[staticmethod]
-    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
-        from_bytes::<_, nucypher_core::E2EThresholdDecryptionRequest>(data)
-    }
-
-    fn __bytes__(&self) -> PyObject {
-        to_bytes(self)
-    }
-}
-
-//
 // EncryptedThresholdDecryptionRequest
 //
 
 #[pyclass(module = "nucypher_core")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct EncryptedThresholdDecryptionRequest {
     backend: nucypher_core::EncryptedThresholdDecryptionRequest,
 }
 
 #[pymethods]
 impl EncryptedThresholdDecryptionRequest {
     #[getter]
-    pub fn ritual_id(&self) -> u16 {
+    pub fn ritual_id(&self) -> u32 {
         self.backend.ritual_id
     }
 
-    pub fn decrypt(&self, sk: &SecretKey) -> PyResult<E2EThresholdDecryptionRequest> {
+    #[getter]
+    pub fn requester_public_key(&self) -> SessionStaticKey {
+        self.backend.requester_public_key.into()
+    }
+
+    pub fn decrypt(
+        &self,
+        shared_secret: &SessionSharedSecret,
+    ) -> PyResult<ThresholdDecryptionRequest> {
         self.backend
-            .decrypt(sk.as_ref())
-            .map(E2EThresholdDecryptionRequest::from)
+            .decrypt(shared_secret.as_ref())
+            .map(ThresholdDecryptionRequest::from)
             .map_err(|err| PyValueError::new_err(format!("{}", err)))
     }
 
     #[staticmethod]
     pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
         from_bytes::<_, nucypher_core::EncryptedThresholdDecryptionRequest>(data)
     }
@@ -807,28 +895,36 @@
 pub struct ThresholdDecryptionResponse {
     backend: nucypher_core::ThresholdDecryptionResponse,
 }
 
 #[pymethods]
 impl ThresholdDecryptionResponse {
     #[new]
-    pub fn new(decryption_share: &[u8]) -> Self {
+    pub fn new(ritual_id: u32, decryption_share: &[u8]) -> Self {
         ThresholdDecryptionResponse {
-            backend: nucypher_core::ThresholdDecryptionResponse::new(decryption_share),
+            backend: nucypher_core::ThresholdDecryptionResponse::new(ritual_id, decryption_share),
         }
     }
 
     #[getter]
+    pub fn ritual_id(&self) -> u32 {
+        self.backend.ritual_id
+    }
+
+    #[getter]
     pub fn decryption_share(&self) -> &[u8] {
         self.backend.decryption_share.as_ref()
     }
 
-    pub fn encrypt(&self, encrypting_key: &PublicKey) -> EncryptedThresholdDecryptionResponse {
+    pub fn encrypt(
+        &self,
+        shared_secret: &SessionSharedSecret,
+    ) -> EncryptedThresholdDecryptionResponse {
         EncryptedThresholdDecryptionResponse {
-            backend: self.backend.encrypt(encrypting_key.as_ref()),
+            backend: self.backend.encrypt(shared_secret.as_ref()),
         }
     }
 
     #[staticmethod]
     pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
         from_bytes::<_, nucypher_core::ThresholdDecryptionResponse>(data)
     }
@@ -846,17 +942,25 @@
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct EncryptedThresholdDecryptionResponse {
     backend: nucypher_core::EncryptedThresholdDecryptionResponse,
 }
 
 #[pymethods]
 impl EncryptedThresholdDecryptionResponse {
-    pub fn decrypt(&self, sk: &SecretKey) -> PyResult<ThresholdDecryptionResponse> {
+    #[getter]
+    pub fn ritual_id(&self) -> u32 {
+        self.backend.ritual_id
+    }
+
+    pub fn decrypt(
+        &self,
+        shared_secret: &SessionSharedSecret,
+    ) -> PyResult<ThresholdDecryptionResponse> {
         self.backend
-            .decrypt(sk.as_ref())
+            .decrypt(shared_secret.as_ref())
             .map(ThresholdDecryptionResponse::from)
             .map_err(|err| PyValueError::new_err(format!("{}", err)))
     }
 
     #[staticmethod]
     pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
         from_bytes::<_, nucypher_core::EncryptedThresholdDecryptionResponse>(data)
@@ -1004,28 +1108,28 @@
     #[new]
     pub fn new(
         staking_provider_address: &Address,
         domain: &str,
         timestamp_epoch: u32,
         verifying_key: &PublicKey,
         encrypting_key: &PublicKey,
-        ferveo_public_key: &[u8], // TODO use ferveo PublicKey type
+        ferveo_public_key: &FerveoPublicKey,
         certificate_der: &[u8],
         host: &str,
         port: u16,
         operator_signature: &RecoverableSignature,
     ) -> PyResult<Self> {
         Ok(Self {
             backend: nucypher_core::NodeMetadataPayload {
                 staking_provider_address: staking_provider_address.backend,
                 domain: domain.to_string(),
                 timestamp_epoch,
                 verifying_key: *verifying_key.as_ref(),
                 encrypting_key: *encrypting_key.as_ref(),
-                ferveo_public_key: ferveo_public_key.into(),
+                ferveo_public_key: *ferveo_public_key.as_ref(),
                 certificate_der: certificate_der.into(),
                 host: host.to_string(),
                 port,
                 operator_signature: operator_signature.as_ref().clone(),
             },
         })
     }
@@ -1044,16 +1148,16 @@
 
     #[getter]
     fn encrypting_key(&self) -> PublicKey {
         self.backend.encrypting_key.into()
     }
 
     #[getter]
-    fn ferveo_public_key(&self) -> &[u8] {
-        self.backend.ferveo_public_key.as_ref()
+    fn ferveo_public_key(&self) -> FerveoPublicKey {
+        self.backend.ferveo_public_key.into()
     }
 
     #[getter]
     fn operator_signature(&self) -> RecoverableSignature {
         self.backend.operator_signature.clone().into()
     }
 
@@ -1309,39 +1413,43 @@
     fn __bytes__(&self) -> PyObject {
         to_bytes(self)
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn _nucypher_core(py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_class::<Address>()?;
-    m.add_class::<Conditions>()?;
-    m.add_class::<Context>()?;
-    m.add_class::<MessageKit>()?;
-    m.add_class::<HRAC>()?;
-    m.add_class::<EncryptedKeyFrag>()?;
-    m.add_class::<TreasureMap>()?;
-    m.add_class::<EncryptedTreasureMap>()?;
-    m.add_class::<ReencryptionRequest>()?;
-    m.add_class::<ReencryptionResponse>()?;
-    m.add_class::<RetrievalKit>()?;
-    m.add_class::<RevocationOrder>()?;
-    m.add_class::<NodeMetadata>()?;
-    m.add_class::<NodeMetadataPayload>()?;
-    m.add_class::<FleetStateChecksum>()?;
-    m.add_class::<MetadataRequest>()?;
-    m.add_class::<MetadataResponsePayload>()?;
-    m.add_class::<MetadataResponse>()?;
-    m.add_class::<ThresholdDecryptionRequest>()?;
-    m.add_class::<E2EThresholdDecryptionRequest>()?;
-    m.add_class::<ThresholdDecryptionResponse>()?;
-    m.add_class::<EncryptedThresholdDecryptionRequest>()?;
-    m.add_class::<EncryptedThresholdDecryptionResponse>()?;
+fn _nucypher_core(py: Python, core_module: &PyModule) -> PyResult<()> {
+    core_module.add_class::<Address>()?;
+    core_module.add_class::<Conditions>()?;
+    core_module.add_class::<Context>()?;
+    core_module.add_class::<MessageKit>()?;
+    core_module.add_class::<HRAC>()?;
+    core_module.add_class::<EncryptedKeyFrag>()?;
+    core_module.add_class::<TreasureMap>()?;
+    core_module.add_class::<EncryptedTreasureMap>()?;
+    core_module.add_class::<ReencryptionRequest>()?;
+    core_module.add_class::<ReencryptionResponse>()?;
+    core_module.add_class::<RetrievalKit>()?;
+    core_module.add_class::<RevocationOrder>()?;
+    core_module.add_class::<NodeMetadata>()?;
+    core_module.add_class::<NodeMetadataPayload>()?;
+    core_module.add_class::<FleetStateChecksum>()?;
+    core_module.add_class::<MetadataRequest>()?;
+    core_module.add_class::<MetadataResponsePayload>()?;
+    core_module.add_class::<MetadataResponse>()?;
+    core_module.add_class::<ThresholdDecryptionRequest>()?;
+    core_module.add_class::<ThresholdDecryptionResponse>()?;
+    core_module.add_class::<EncryptedThresholdDecryptionRequest>()?;
+    core_module.add_class::<EncryptedThresholdDecryptionResponse>()?;
+    core_module.add_class::<SessionSharedSecret>()?;
+    core_module.add_class::<SessionStaticKey>()?;
+    core_module.add_class::<SessionStaticSecret>()?;
+    core_module.add_class::<SessionSecretFactory>()?;
 
+    // Build the umbral module
     let umbral_module = PyModule::new(py, "umbral")?;
 
     umbral_module.add_class::<umbral_pre::bindings_python::SecretKey>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::SecretKeyFactory>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::PublicKey>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::Capsule>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::VerifiedKeyFrag>()?;
@@ -1357,11 +1465,16 @@
     umbral_module.add_class::<umbral_pre::bindings_python::ReencryptionEvidence>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::CurvePoint>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::Parameters>()?;
     umbral_module.add(
         "VerificationError",
         py.get_type::<umbral_pre::bindings_python::VerificationError>(),
     )?; // depends on what `reencryption_response.verify()` returns
-    m.add_submodule(umbral_module)?;
+    core_module.add_submodule(umbral_module)?;
+
+    // Build the ferveo module
+    let ferveo_module = PyModule::new(py, "ferveo")?;
+    ferveo::bindings_python::make_ferveo_py_module(py, ferveo_module)?;
+    core_module.add_submodule(ferveo_module)?;
 
     Ok(())
 }
```

