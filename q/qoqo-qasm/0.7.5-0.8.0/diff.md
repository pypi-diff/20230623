# Comparing `tmp/qoqo_qasm-0.7.5.tar.gz` & `tmp/qoqo_qasm-0.8.0.tar.gz`

## Comparing `qoqo_qasm-0.7.5.tar` & `qoqo_qasm-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/LICENSE
--rw-r--r--   0     1001      123     2618 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/README.md
--rw-r--r--   0     1001      123    10787 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/src/backend.rs
--rw-r--r--   0     1001      123    44935 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/src/interface.rs
--rw-r--r--   0     1001      123     1112 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/src/lib.rs
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 qoqo_qasm-0.7.5/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/LICENSE
--rw-r--r--   0     1001      123     2618 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/README.md
--rw-r--r--   0     1001      123      701 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/build.rs
--rw-r--r--   0     1001      123      728 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/pyproject.toml
--rw-r--r--   0     1001      123       87 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/python_tests/README.md
--rw-r--r--   0     1001      123   957096 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/qoqo_qasm/DEPENDENCIES
--rw-r--r--   0     1001      123      916 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/qoqo_qasm/__init__.py
--rw-r--r--   0     1001      123     4282 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/src/backend.rs
--rw-r--r--   0     1001      123     3707 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/src/interface.rs
--rw-r--r--   0     1001      123     1443 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/src/lib.rs
--rw-r--r--   0     1001      123    20511 2023-06-01 14:48:11.000000 qoqo_qasm-0.7.5/Cargo.lock
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 qoqo_qasm-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/LICENSE
+-rw-r--r--   0     1001      123     2621 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/README.md
+-rw-r--r--   0     1001      123    11723 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/backend.rs
+-rw-r--r--   0     1001      123      875 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/grammars/qasm2_0.pest
+-rw-r--r--   0     1001      123    44935 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/interface.rs
+-rw-r--r--   0     1001      123     1367 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/lib.rs
+-rw-r--r--   0     1001      123    12539 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/parser.rs
+-rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.0/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/LICENSE
+-rw-r--r--   0     1001      123     2621 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/README.md
+-rw-r--r--   0     1001      123      701 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/build.rs
+-rw-r--r--   0     1001      123      728 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/pyproject.toml
+-rw-r--r--   0     1001      123       87 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/python_tests/README.md
+-rw-r--r--   0     1001      123   957096 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/qoqo_qasm/DEPENDENCIES
+-rw-r--r--   0     1001      123      916 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/qoqo_qasm/__init__.py
+-rw-r--r--   0     1001      123     5419 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/src/backend.rs
+-rw-r--r--   0     1001      123     3707 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/src/interface.rs
+-rw-r--r--   0     1001      123     1796 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/src/lib.rs
+-rw-r--r--   0     1001      123     2134 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/src/parser.rs
+-rw-r--r--   0     1001      123    23186 2023-06-23 12:30:42.000000 qoqo_qasm-0.8.0/Cargo.lock
+-rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 qoqo_qasm-0.8.0/PKG-INFO
```

### Comparing `qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/Cargo.toml` & `qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo-qasm"
-version = "0.7.5"
+version = "0.8.0"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2018"
 categories = ["science", "simulation"]
 readme = "README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qasm"
 description = "QASM interface for roqoqo rust quantum computing toolkit"
@@ -14,10 +14,16 @@
 name = "roqoqo_qasm"
 path = "src/lib.rs"
 doctest = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-roqoqo = { version = "1.4", features = ["serialize"] }
+roqoqo = { version = "1.5", features = ["serialize"] }
 qoqo_calculator = { version = "1.1" }
 ndarray = "0.15"
+pest = { version = "2.5", optional = true }
+pest_derive = { version = "2.5", optional = true }
+num-complex = "0.4"
+
+[features]
+unstable_qasm_import = ["pest", "pest_derive"]
```

### Comparing `qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/LICENSE` & `qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/README.md` & `qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
+<img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo-qasm
 
 Qasm interface for the qoqo/roqoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
 
 This repository contains two components:
```

### Comparing `qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/src/backend.rs` & `qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -247,38 +247,66 @@
         circuit: &Circuit,
         folder_name: &Path,
         filename: &Path,
         overwrite: bool,
     ) -> Result<(), RoqoqoBackendError> {
         self.circuit_iterator_to_qasm_file(circuit.iter(), folder_name, filename, overwrite)
     }
+
+    /// Translates a QASM file into a qoqo Circuit instance.
+    ///
+    /// # Arguments
+    ///
+    /// * `file` - The '.qasm' file to translate.
+    ///
+    /// # Returns
+    ///
+    /// * `Ok(Circuit)` - The translated qoqo Circuit.
+    /// * `RoqoqoBackendError::GenericError` - Error encountered while parsing.
+    #[cfg(feature = "unstable_qasm_import")]
+    pub fn file_to_circuit(&self, file: File) -> Result<Circuit, RoqoqoBackendError> {
+        crate::file_to_circuit(file)
+    }
+
+    /// Translates a QASM string into a qoqo Circuit instance.
+    ///
+    /// # Arguments
+    ///
+    /// * `input` - The QASM string to translate.
+    ///
+    /// # Returns
+    ///
+    /// * `Ok(Circuit)` - The translated qoqo Circuit.
+    /// * `RoqoqoBackendError::GenericError` - Error encountered while parsing.
+    #[cfg(feature = "unstable_qasm_import")]
+    pub fn string_to_circuit(&self, input: &str) -> Result<Circuit, RoqoqoBackendError> {
+        crate::string_to_circuit(input)
+    }
 }
 
 /// Enum for setting the version of OpenQASM used
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub enum QasmVersion {
     /// OpenQASM 2.0
     V2point0,
     /// OpenQASM 3.0
     V3point0(Qasm3Dialect),
 }
 
 /// Enum for setting the version of OpenQASM used
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub enum Qasm3Dialect {
-    /// OpenQASM 2.0 FIX
+    /// No Pragma operations
     Vanilla,
-    /// OpenQASM 3.0 FIX
+    /// With Pragma operations
     Roqoqo,
-    /// OpenQASM 3.0 FIX
+    /// With Braket's Pragma operations
     Braket,
 }
 
-// v3point0 => vanilla, no pragmas; roqoqo, our pragmas; braket, braket pragmas
-
 impl FromStr for QasmVersion {
     type Err = RoqoqoBackendError;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         match s {
             "2.0" => Ok(QasmVersion::V2point0),
             "3.0Roqoqo" => Ok(QasmVersion::V3point0(Qasm3Dialect::Roqoqo)),
```

### Comparing `qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/src/interface.rs` & `qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/interface.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.7.5/local_dependencies/roqoqo-qasm/src/lib.rs` & `qoqo_qasm-0.8.0/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -13,17 +13,38 @@
 #![deny(missing_docs)]
 #![warn(rustdoc::private_intra_doc_links)]
 #![warn(rustdoc::missing_crate_level_docs)]
 #![warn(rustdoc::missing_doc_code_examples)]
 #![warn(rustdoc::private_doc_tests)]
 #![deny(missing_debug_implementations)]
 
-//! # roqoqo-qasm
+//! # qoqo-qasm
 //!
 //! QASM interface for qoqo.
 //!
 //! Translates qoqo operations and circuits to QASM operations via the interface, and Create a Qasm file with QasmBackend.
 
+use pyo3::prelude::*;
+use pyo3::wrap_pyfunction;
+
 mod backend;
 pub use backend::*;
+
 mod interface;
 pub use interface::*;
+
+#[cfg(feature = "unstable_qasm_import")]
+mod parser;
+#[cfg(feature = "unstable_qasm_import")]
+pub use parser::*;
+
+#[pymodule]
+fn qoqo_qasm(_py: Python, module: &PyModule) -> PyResult<()> {
+    module.add_class::<QasmBackendWrapper>()?;
+    module.add_function(wrap_pyfunction!(qasm_call_circuit, module)?)?;
+    module.add_function(wrap_pyfunction!(qasm_call_operation, module)?)?;
+    #[cfg(feature = "unstable_qasm_import")]
+    module.add_function(wrap_pyfunction!(qasm_file_to_circuit, module)?)?;
+    #[cfg(feature = "unstable_qasm_import")]
+    module.add_function(wrap_pyfunction!(qasm_str_to_circuit, module)?)?;
+    Ok(())
+}
```

### Comparing `qoqo_qasm-0.7.5/Cargo.toml` & `qoqo_qasm-0.8.0/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 [package]
 name = "qoqo_qasm"
-version = "0.7.5"
+version = "0.8.0"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2018"
 categories = ["science", "simulation"]
 readme = "README.md"
 homepage = "https://github.com/HQSquantumsimulations/qoqo_qasm"
 repository = "https://github.com/HQSquantumsimulations/qoqo_qasm"
 description = "Python interface of roqoqo mocked backend"
-include = ["src*", "build.rs", "qoqo_qasm", "LICENSE", "pyproject.toml", "README.md"]
+include = [
+    "src*",
+    "build.rs",
+    "qoqo_qasm",
+    "LICENSE",
+    "pyproject.toml",
+    "README.md",
+]
 
 [lib]
 name = "qoqo_qasm"
 path = "src/lib.rs"
 doctest = false
 crate-type = ["cdylib", "rlib"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-qoqo = {version="1.4", default-features = false}
-roqoqo = {version="1.4", features=["serialize"]}
-roqoqo-qasm = { version = "0.7", path = "local_dependencies/roqoqo-qasm" }
+qoqo = { version = "1.5", default-features = false }
+roqoqo = { version = "1.5", features = ["serialize"] }
+roqoqo-qasm = { version = "0.8", path = "local_dependencies/roqoqo-qasm" }
 
 [dependencies.pyo3]
 version = "0.18"
 features = ["num-complex"]
 
 [build-dependencies]
 pyo3-build-config = "0.18"
 
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
+unstable_qasm_import = ["roqoqo-qasm/unstable_qasm_import"]
```

### Comparing `qoqo_qasm-0.7.5/LICENSE` & `qoqo_qasm-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.7.5/README.md` & `qoqo_qasm-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
+<img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo-qasm
 
 Qasm interface for the qoqo/roqoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
 
 This repository contains two components:
```

### Comparing `qoqo_qasm-0.7.5/build.rs` & `qoqo_qasm-0.8.0/build.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.7.5/pyproject.toml` & `qoqo_qasm-0.8.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "qoqo_qasm"
-version = "0.7.5"
+version = "0.8.0"
 dependencies = [
-  'qoqo>=1.4',
+  'qoqo>=1.5',
   'qoqo_calculator_pyo3>=1.1',
 ]
 license = {text="Apache-2.0 AND Apache-2.0 with LLVM-exception AND MIT AND Unicode-DFS-2016 AND BSD-2-Clause AND BSD-3-CLause"}
 maintainers = [{name = "HQS Quantum Simulations GmbH", email = "info@quantumsimulations.de"}]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
```

### Comparing `qoqo_qasm-0.7.5/qoqo_qasm/DEPENDENCIES` & `qoqo_qasm-0.8.0/qoqo_qasm/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -16203,15 +16203,15 @@
 0003f4a0: 4456 4953 4544 204f 4620 5448 4520 504f  DVISED OF THE PO
 0003f4b0: 5353 4942 494c 4954 5920 4f46 2053 5543  SSIBILITY OF SUC
 0003f4c0: 4820 4441 4d41 4745 2e0a 0a0a 3d3d 3d3d  H DAMAGE....====
 0003f4d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003f4e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003f4f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003f500: 0a6f 6e63 655f 6365 6c6c 2031 2e31 372e  .once_cell 1.17.
-0003f510: 310a 6874 7470 733a 2f2f 6769 7468 7562  1.https://github
+0003f510: 320a 6874 7470 733a 2f2f 6769 7468 7562  2.https://github
 0003f520: 2e63 6f6d 2f6d 6174 6b6c 6164 2f6f 6e63  .com/matklad/onc
 0003f530: 655f 6365 6c6c 0a62 7920 416c 656b 7365  e_cell.by Alekse
 0003f540: 7920 4b6c 6164 6f76 203c 616c 656b 7365  y Kladov <alekse
 0003f550: 792e 6b6c 6164 6f76 4067 6d61 696c 2e63  y.kladov@gmail.c
 0003f560: 6f6d 3e0a 5369 6e67 6c65 2061 7373 6967  om>.Single assig
 0003f570: 6e6d 656e 7420 6365 6c6c 7320 616e 6420  nment cells and 
 0003f580: 6c61 7a79 2076 616c 7565 732e 0a4c 6963  lazy values..Lic
@@ -22289,15 +22289,15 @@
 00057100: 4520 5553 4520 4f52 204f 5448 4552 2044  E USE OR OTHER D
 00057110: 4541 4c49 4e47 5320 494e 2054 4845 0a53  EALINGS IN THE.S
 00057120: 4f46 5457 4152 452e 0a0a 0a3d 3d3d 3d3d  OFTWARE....=====
 00057130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00057140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00057150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
 00057160: 7072 6f63 2d6d 6163 726f 3220 312e 302e  proc-macro2 1.0.
-00057170: 3538 0a68 7474 7073 3a2f 2f67 6974 6875  58.https://githu
+00057170: 3539 0a68 7474 7073 3a2f 2f67 6974 6875  59.https://githu
 00057180: 622e 636f 6d2f 6474 6f6c 6e61 792f 7072  b.com/dtolnay/pr
 00057190: 6f63 2d6d 6163 726f 320a 6279 2044 6176  oc-macro2.by Dav
 000571a0: 6964 2054 6f6c 6e61 7920 3c64 746f 6c6e  id Tolnay <dtoln
 000571b0: 6179 4067 6d61 696c 2e63 6f6d 3e2c 2041  ay@gmail.com>, A
 000571c0: 6c65 7820 4372 6963 6874 6f6e 203c 616c  lex Crichton <al
 000571d0: 6578 4061 6c65 7863 7269 6368 746f 6e2e  ex@alexcrichton.
 000571e0: 636f 6d3e 0a41 2073 7562 7374 6974 7574  com>.A substitut
@@ -27677,15 +27677,15 @@
 0006c1c0: 6f66 2079 6f75 7220 6163 6365 7074 696e  of your acceptin
 0006c1d0: 6720 616e 7920 7375 6368 2077 6172 7261  g any such warra
 0006c1e0: 6e74 7920 6f72 2061 6464 6974 696f 6e61  nty or additiona
 0006c1f0: 6c20 6c69 6162 696c 6974 792e 0a0a 0a3d  l liability....=
 0006c200: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0006c210: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0006c220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0006c230: 3d3d 3d0a 716f 716f 2031 2e34 2e30 0a68  ===.qoqo 1.4.0.h
+0006c230: 3d3d 3d0a 716f 716f 2031 2e35 2e30 0a68  ===.qoqo 1.5.0.h
 0006c240: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 0006c250: 6d2f 4851 5371 7561 6e74 756d 7369 6d75  m/HQSquantumsimu
 0006c260: 6c61 7469 6f6e 732f 716f 716f 0a62 7920  lations/qoqo.by 
 0006c270: 4851 5320 5175 616e 7475 6d20 5369 6d75  HQS Quantum Simu
 0006c280: 6c61 7469 6f6e 7320 3c69 6e66 6f40 7175  lations <info@qu
 0006c290: 616e 7475 6d73 696d 756c 6174 696f 6e73  antumsimulations
 0006c2a0: 2e64 653e 0a51 7561 6e74 756d 2063 6f6d  .de>.Quantum com
@@ -28407,15 +28407,15 @@
 0006ef60: 6572 6e69 6e67 2070 6572 6d69 7373 696f  erning permissio
 0006ef70: 6e73 2061 6e64 0a20 2020 6c69 6d69 7461  ns and.   limita
 0006ef80: 7469 6f6e 7320 756e 6465 7220 7468 6520  tions under the 
 0006ef90: 4c69 6365 6e73 652e 0a0a 0a3d 3d3d 3d3d  License....=====
 0006efa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0006efb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0006efc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-0006efd0: 716f 716f 2d6d 6163 726f 7320 312e 342e  qoqo-macros 1.4.
+0006efd0: 716f 716f 2d6d 6163 726f 7320 312e 352e  qoqo-macros 1.5.
 0006efe0: 300a 6279 2048 5153 2051 7561 6e74 756d  0.by HQS Quantum
 0006eff0: 2053 696d 756c 6174 696f 6e73 203c 696e   Simulations <in
 0006f000: 666f 4071 7561 6e74 756d 7369 6d75 6c61  fo@quantumsimula
 0006f010: 7469 6f6e 732e 6465 3e0a 4d61 6372 6f73  tions.de>.Macros
 0006f020: 2066 6f72 2074 6865 2071 6f71 6f20 6372   for the qoqo cr
 0006f030: 6174 650a 4c69 6365 6e73 653a 2041 7061  ate.License: Apa
 0006f040: 6368 652d 322e 300a 2d2d 2d2d 2d2d 2d2d  che-2.0.--------
@@ -31330,15 +31330,15 @@
 0007a610: 696e 6720 7065 726d 6973 7369 6f6e 7320  ing permissions 
 0007a620: 616e 640a 2020 206c 696d 6974 6174 696f  and.   limitatio
 0007a630: 6e73 2075 6e64 6572 2074 6865 204c 6963  ns under the Lic
 0007a640: 656e 7365 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d  ense....========
 0007a650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0007a660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0007a670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a71 756f  ============.quo
-0007a680: 7465 2031 2e30 2e32 370a 6874 7470 733a  te 1.0.27.https:
+0007a680: 7465 2031 2e30 2e32 380a 6874 7470 733a  te 1.0.28.https:
 0007a690: 2f2f 6769 7468 7562 2e63 6f6d 2f64 746f  //github.com/dto
 0007a6a0: 6c6e 6179 2f71 756f 7465 0a62 7920 4461  lnay/quote.by Da
 0007a6b0: 7669 6420 546f 6c6e 6179 203c 6474 6f6c  vid Tolnay <dtol
 0007a6c0: 6e61 7940 676d 6169 6c2e 636f 6d3e 0a51  nay@gmail.com>.Q
 0007a6d0: 7561 7369 2d71 756f 7469 6e67 206d 6163  uasi-quoting mac
 0007a6e0: 726f 2071 756f 7465 2128 2e2e 2e29 0a4c  ro quote!(...).L
 0007a6f0: 6963 656e 7365 3a20 4d49 5420 4f52 2041  icense: MIT OR A
@@ -35823,15 +35823,15 @@
 0008bee0: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
 0008bef0: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
 0008bf00: 414c 494e 4753 2049 4e20 5448 4520 534f  ALINGS IN THE SO
 0008bf10: 4654 5741 5245 2e0a 0a0a 3d3d 3d3d 3d3d  FTWARE....======
 0008bf20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0008bf30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0008bf40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a72  ==============.r
-0008bf50: 6f71 6f71 6f20 312e 342e 300a 6874 7470  oqoqo 1.4.0.http
+0008bf50: 6f71 6f71 6f20 312e 352e 300a 6874 7470  oqoqo 1.5.0.http
 0008bf60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f48  s://github.com/H
 0008bf70: 5153 7175 616e 7475 6d73 696d 756c 6174  QSquantumsimulat
 0008bf80: 696f 6e73 2f71 6f71 6f0a 6279 2048 5153  ions/qoqo.by HQS
 0008bf90: 2051 7561 6e74 756d 2053 696d 756c 6174   Quantum Simulat
 0008bfa0: 696f 6e73 203c 696e 666f 4071 7561 6e74  ions <info@quant
 0008bfb0: 756d 7369 6d75 6c61 7469 6f6e 732e 6465  umsimulations.de
 0008bfc0: 3e0a 5275 7374 2051 7561 6e74 756d 2043  >.Rust Quantum C
@@ -36552,15 +36552,15 @@
 0008ec70: 6973 7369 6f6e 7320 616e 640a 2020 206c  issions and.   l
 0008ec80: 696d 6974 6174 696f 6e73 2075 6e64 6572  imitations under
 0008ec90: 2074 6865 204c 6963 656e 7365 2e0a 0a0a   the License....
 0008eca0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0008ecb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0008ecc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0008ecd0: 3d3d 3d3d 0a72 6f71 6f71 6f2d 6465 7269  ====.roqoqo-deri
-0008ece0: 7665 2031 2e34 2e30 0a62 7920 4851 5320  ve 1.4.0.by HQS 
+0008ece0: 7665 2031 2e35 2e30 0a62 7920 4851 5320  ve 1.5.0.by HQS 
 0008ecf0: 5175 616e 7475 6d20 5369 6d75 6c61 7469  Quantum Simulati
 0008ed00: 6f6e 7320 3c69 6e66 6f40 7175 616e 7475  ons <info@quantu
 0008ed10: 6d73 696d 756c 6174 696f 6e73 2e64 653e  msimulations.de>
 0008ed20: 0a4d 6163 726f 7320 666f 7220 7468 6520  .Macros for the 
 0008ed30: 726f 716f 716f 2063 7261 7465 0a4c 6963  roqoqo crate.Lic
 0008ed40: 656e 7365 3a20 4170 6163 6865 2d32 2e30  ense: Apache-2.0
 0008ed50: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
@@ -44681,15 +44681,15 @@
 000ae880: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
 000ae890: 4f52 204f 5448 4552 0a44 4541 4c49 4e47  OR OTHER.DEALING
 000ae8a0: 5320 494e 2054 4845 2053 4f46 5457 4152  S IN THE SOFTWAR
 000ae8b0: 452e 0a0a 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  E....===========
 000ae8c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000ae8d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000ae8e0: 3d3d 3d3d 3d3d 3d3d 3d0a 7379 6e20 322e  =========.syn 2.
-000ae8f0: 302e 3136 0a68 7474 7073 3a2f 2f67 6974  0.16.https://git
+000ae8f0: 302e 3138 0a68 7474 7073 3a2f 2f67 6974  0.18.https://git
 000ae900: 6875 622e 636f 6d2f 6474 6f6c 6e61 792f  hub.com/dtolnay/
 000ae910: 7379 6e0a 6279 2044 6176 6964 2054 6f6c  syn.by David Tol
 000ae920: 6e61 7920 3c64 746f 6c6e 6179 4067 6d61  nay <dtolnay@gma
 000ae930: 696c 2e63 6f6d 3e0a 5061 7273 6572 2066  il.com>.Parser f
 000ae940: 6f72 2052 7573 7420 736f 7572 6365 2063  or Rust source c
 000ae950: 6f64 650a 4c69 6365 6e73 653a 204d 4954  ode.License: MIT
 000ae960: 204f 5220 4170 6163 6865 2d32 2e30 0a2d   OR Apache-2.0.-
@@ -48615,15 +48615,15 @@
 000bde60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000bde70: 2d0a 4c49 4345 4e53 453a 0a0a 4d49 5420  -.LICENSE:..MIT 
 000bde80: 4f52 2041 7061 6368 652d 322e 300a 0a3d  OR Apache-2.0..=
 000bde90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000bdea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000bdeb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000bdec0: 3d3d 3d0a 756e 6963 6f64 652d 6964 656e  ===.unicode-iden
-000bded0: 7420 312e 302e 380a 6874 7470 733a 2f2f  t 1.0.8.https://
+000bded0: 7420 312e 302e 390a 6874 7470 733a 2f2f  t 1.0.9.https://
 000bdee0: 6769 7468 7562 2e63 6f6d 2f64 746f 6c6e  github.com/dtoln
 000bdef0: 6179 2f75 6e69 636f 6465 2d69 6465 6e74  ay/unicode-ident
 000bdf00: 0a62 7920 4461 7669 6420 546f 6c6e 6179  .by David Tolnay
 000bdf10: 203c 6474 6f6c 6e61 7940 676d 6169 6c2e   <dtolnay@gmail.
 000bdf20: 636f 6d3e 0a44 6574 6572 6d69 6e65 2077  com>.Determine w
 000bdf30: 6865 7468 6572 2063 6861 7261 6374 6572  hether character
 000bdf40: 7320 6861 7665 2074 6865 2058 4944 5f53  s have the XID_S
```

### Comparing `qoqo_qasm-0.7.5/qoqo_qasm/__init__.py` & `qoqo_qasm-0.8.0/qoqo_qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.7.5/src/backend.rs` & `qoqo_qasm-0.8.0/src/backend.rs`

 * *Files 22% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 // express or implied. See the License for the specific language governing permissions and
 // limitations under the License.
 
 use pyo3::{
     exceptions::{PyTypeError, PyValueError},
     prelude::*,
 };
+use std::path::Path;
+
 use qoqo::convert_into_circuit;
+#[cfg(feature = "unstable_qasm_import")]
+use qoqo::CircuitWrapper;
+
 use roqoqo_qasm::Backend;
-use std::path::Path;
 
 /// Backend to qoqo that produces QASM output which can be imported.
 ///
 /// This backend takes a qoqo circuit to be run on a certain device and returns a QASM file
 /// containing the translated circuit. The circuit itself is translated using the qoqo_qasm
 /// interface. In this backend, the initialization sets up the relevant parameters and the run
 /// function calls the QASM interface and writes the QASM file, which is saved to be used by the
@@ -65,15 +69,15 @@
     ///     TypeError: Circuit conversion error
     ///     ValueError: Operation not in QASM backend
     #[pyo3(text_signature = "($self, circuit)")]
     pub fn circuit_to_qasm_str(&self, circuit: &PyAny) -> PyResult<String> {
         let circuit = convert_into_circuit(circuit).map_err(|x| {
             PyTypeError::new_err(format!("Cannot convert python object to Circuit: {x:?}"))
         })?;
-        roqoqo_qasm::Backend::circuit_to_qasm_str(&self.internal, &circuit)
+        Backend::circuit_to_qasm_str(&self.internal, &circuit)
             .map_err(|x| PyValueError::new_err(format!("Error during QASM translation: {x:?}")))
     }
 
     /// Translates a Circuit to a QASM file.
     ///
     /// Args:
     ///     circuit: The Circuit that is translated
@@ -96,17 +100,44 @@
         overwrite: bool,
     ) -> PyResult<()> {
         let circuit = convert_into_circuit(circuit).map_err(|x| {
             PyTypeError::new_err(format!("Cannot convert python object to Circuit: {x:?}"))
         })?;
         let folder_name = Path::new(&folder_name);
         let filename = Path::new(&filename);
-        roqoqo_qasm::Backend::circuit_to_qasm_file(
-            &self.internal,
-            &circuit,
-            folder_name,
-            filename,
-            overwrite,
-        )
-        .map_err(|x| PyValueError::new_err(format!("Error during QASM translation: {x:?}")))
+        Backend::circuit_to_qasm_file(&self.internal, &circuit, folder_name, filename, overwrite)
+            .map_err(|x| PyValueError::new_err(format!("Error during QASM translation: {x:?}")))
+    }
+
+    /// Translates a QASM File to a Circuit.
+    ///
+    /// Args:
+    ///     file (str): The path to the QASM file.
+    ///
+    /// Returns:
+    ///     Circuit: The Circuit that was read from the QASM file.
+    ///
+    /// Raises:
+    ///     PyFileNotFoundError: The file could not be opened.
+    ///     PyValueError: An error occurred while converting the file into a Circuit.
+    #[cfg(feature = "unstable_qasm_import")]
+    #[pyo3(text_signature = "($self, file)")]
+    pub fn qasm_file_to_circuit(&self, file: &str) -> PyResult<CircuitWrapper> {
+        crate::qasm_file_to_circuit(file)
+    }
+
+    /// Translates a QASM string into a qoqo Circuit instance.
+    ///
+    /// Args:
+    ///     input (str): The QASM string to translate.
+    ///
+    /// Returns:
+    ///     Circuit: The Circuit that was read from the QASM file.
+    ///
+    /// Raises:
+    ///     PyValueError: An error occurred while converting the file into a Circuit.
+    #[cfg(feature = "unstable_qasm_import")]
+    #[pyo3(text_signature = "(input)")]
+    pub fn qasm_str_to_circuit(&self, input: &str) -> PyResult<CircuitWrapper> {
+        crate::qasm_str_to_circuit(input)
     }
 }
```

### Comparing `qoqo_qasm-0.7.5/src/interface.rs` & `qoqo_qasm-0.8.0/src/interface.rs`

 * *Files identical despite different names*

### Comparing `qoqo_qasm-0.7.5/src/lib.rs` & `qoqo_qasm-0.8.0/local_dependencies/roqoqo-qasm/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -6,36 +6,34 @@
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software distributed under the
 // License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 // express or implied. See the License for the specific language governing permissions and
 // limitations under the License.
 
-#![deny(missing_docs)]
+#![allow(missing_docs)]
 #![warn(rustdoc::private_intra_doc_links)]
 #![warn(rustdoc::missing_crate_level_docs)]
 #![warn(rustdoc::missing_doc_code_examples)]
 #![warn(rustdoc::private_doc_tests)]
 #![deny(missing_debug_implementations)]
 
-//! # qoqo-qasm
+//! # roqoqo-qasm
 //!
 //! QASM interface for qoqo.
 //!
 //! Translates qoqo operations and circuits to QASM operations via the interface, and Create a Qasm file with QasmBackend.
 
-use pyo3::prelude::*;
-use pyo3::wrap_pyfunction;
+#[cfg(feature = "unstable_qasm_import")]
+extern crate pest;
+#[macro_use]
+#[cfg(feature = "unstable_qasm_import")]
+extern crate pest_derive;
 
 mod backend;
 pub use backend::*;
-
 mod interface;
 pub use interface::*;
-
-#[pymodule]
-fn qoqo_qasm(_py: Python, module: &PyModule) -> PyResult<()> {
-    module.add_class::<QasmBackendWrapper>()?;
-    module.add_function(wrap_pyfunction!(qasm_call_circuit, module)?)?;
-    module.add_function(wrap_pyfunction!(qasm_call_operation, module)?)?;
-    Ok(())
-}
+#[cfg(feature = "unstable_qasm_import")]
+mod parser;
+#[cfg(feature = "unstable_qasm_import")]
+pub use parser::*;
```

### Comparing `qoqo_qasm-0.7.5/Cargo.lock` & `qoqo_qasm-0.8.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -29,32 +29,80 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "block-buffer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cpufeatures"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "crypto-common"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
+dependencies = [
+ "generic-array",
+ "typenum",
+]
+
+[[package]]
+name = "digest"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
+name = "generic-array"
+version = "0.14.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
+
+[[package]]
 name = "getrandom"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
@@ -259,14 +307,58 @@
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
+name = "pest"
+version = "2.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
+dependencies = [
+ "thiserror",
+ "ucd-trie",
+]
+
+[[package]]
+name = "pest_derive"
+version = "2.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
+dependencies = [
+ "pest",
+ "pest_generator",
+]
+
+[[package]]
+name = "pest_generator"
+version = "2.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
+dependencies = [
+ "pest",
+ "pest_meta",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "pest_meta"
+version = "2.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
+dependencies = [
+ "once_cell",
+ "pest",
+ "sha2",
+]
+
+[[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
  "indexmap",
@@ -372,17 +464,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "qoqo"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf07f3e506270363fc27cd0d64d6a731e16bb541aefe5d6ada33a5eae988abff"
+checksum = "b989a139a4330c99bdf79f77827e5fedd96f3620596211214ea475fd40bc6bdd"
 dependencies = [
  "bincode",
  "ndarray",
  "num-complex",
  "numpy",
  "proc-macro2",
  "pyo3",
@@ -396,17 +488,17 @@
  "serde_json",
  "syn 2.0.18",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo-macros"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d92049ac4baa56a91d6d349714192e8ccb48cbceab7c0ed01a225442e950e492"
+checksum = "03411b76166a46cb3e8e2d6846cefe0c53c77f9d8469a8a4b2224121e34f2761"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -432,15 +524,15 @@
  "qoqo_calculator",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo_qasm"
-version = "0.7.5"
+version = "0.8.0"
 dependencies = [
  "ndarray",
  "pyo3",
  "pyo3-build-config",
  "qoqo",
  "qoqo_calculator",
  "roqoqo",
@@ -510,17 +602,17 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "roqoqo"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64df85d14e330f6ecb7736ef2251cbd86508c50a2edda310edc23054caa76822"
+checksum = "15b5e9d03e8f531c6a9781f8aafff4605609aea622b0121dae5f2b046bb1d0ff"
 dependencies = [
  "bincode",
  "nalgebra",
  "ndarray",
  "num-complex",
  "petgraph",
  "proc-macro2",
@@ -532,28 +624,31 @@
  "serde",
  "syn 2.0.18",
  "thiserror",
 ]
 
 [[package]]
 name = "roqoqo-derive"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74660c4266cc53915499961c19a15e7e558dcce5c39a0c4ea1f3ad41e0dbab44"
+checksum = "fe0bdd70484ec44a5580ecd12ba68bca8dbfe789ca6c87464828b2c8d5355dd6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "roqoqo-qasm"
-version = "0.7.5"
+version = "0.8.0"
 dependencies = [
  "ndarray",
+ "num-complex",
+ "pest",
+ "pest_derive",
  "qoqo_calculator",
  "roqoqo",
  "test-case",
 ]
 
 [[package]]
 name = "rustc-hash"
@@ -610,14 +705,25 @@
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "sha2"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
+
+[[package]]
 name = "simba"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
@@ -718,14 +824,20 @@
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
+name = "ucd-trie"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
```

### Comparing `qoqo_qasm-0.7.5/PKG-INFO` & `qoqo_qasm-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qoqo_qasm
-Version: 0.7.5
-Requires-Dist: qoqo >=1.4
+Version: 0.8.0
+Requires-Dist: qoqo >=1.5
 Requires-Dist: qoqo_calculator_pyo3 >=1.1
 Requires-Dist: tomli ; extra == 'docs'
 Requires-Dist: numpy ; extra == 'docs'
 Requires-Dist: sphinx >=2.1 ; extra == 'docs'
 Requires-Dist: nbsphinx ; extra == 'docs'
 Requires-Dist: pygments ; extra == 'docs'
 Requires-Dist: recommonmark ; extra == 'docs'
@@ -20,15 +20,15 @@
 Maintainer-email: HQS Quantum Simulations GmbH <info@quantumsimulations.de>
 License: Apache-2.0 AND Apache-2.0 with LLVM-exception AND MIT AND Unicode-DFS-2016 AND
 	BSD-2-Clause AND BSD-3-CLause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/HQSquantumsimulations/qoqo_qasm
 
-<img src="qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
+<img src="../qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo-qasm
 
 Qasm interface for the qoqo/roqoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
 
 This repository contains two components:
```

