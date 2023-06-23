# Comparing `tmp/nifpga_fast_fifo_recv-0.99.3.tar.gz` & `tmp/nifpga_fast_fifo_recv-0.99.4.tar.gz`

## Comparing `nifpga_fast_fifo_recv-0.99.3.tar` & `nifpga_fast_fifo_recv-0.99.4.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.3/Cargo.toml
--rw-r--r--   0        0        0     1081 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/LICENSE
--rw-r--r--   0        0        0     5061 2023-06-22 09:57:52.000000 nifpga_fast_fifo_recv-0.99.3/README.md
--rw-r--r--   0        0        0      561 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/pyproject.toml
--rw-r--r--   0        0        0        9 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/requirements.txt
--rw-r--r--   0        0        0     7728 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/src/lib.rs
--rw-r--r--   0        0        0    10405 2023-06-22 09:57:53.000000 nifpga_fast_fifo_recv-0.99.3/Cargo.lock
--rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.3/PKG-INFO
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.4/Cargo.toml
+-rw-r--r--   0        0        0       50 2023-06-21 09:31:01.000000 nifpga_fast_fifo_recv-0.99.4/.idea/.gitignore
+-rw-r--r--   0        0        0      174 2023-06-21 09:31:01.000000 nifpga_fast_fifo_recv-0.99.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      213 2023-06-21 09:31:01.000000 nifpga_fast_fifo_recv-0.99.4/.idea/misc.xml
+-rw-r--r--   0        0        0      301 2023-06-21 09:31:01.000000 nifpga_fast_fifo_recv-0.99.4/.idea/modules.xml
+-rw-r--r--   0        0        0      438 2023-06-21 09:31:01.000000 nifpga_fast_fifo_recv-0.99.4/.idea/nifpga-fast-fifo-recv.iml
+-rw-r--r--   0        0        0      172 2023-06-21 09:31:01.000000 nifpga_fast_fifo_recv-0.99.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     3497 2023-06-22 10:09:03.000000 nifpga_fast_fifo_recv-0.99.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     1081 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.4/LICENSE
+-rw-r--r--   0        0        0     5061 2023-06-22 09:57:52.000000 nifpga_fast_fifo_recv-0.99.4/README.md
+-rw-r--r--   0        0        0      561 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.4/pyproject.toml
+-rw-r--r--   0        0        0        9 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.4/requirements.txt
+-rw-r--r--   0        0        0     7736 2023-06-23 12:46:29.000000 nifpga_fast_fifo_recv-0.99.4/src/lib.rs
+-rw-r--r--   0        0        0    10557 2023-06-23 12:48:06.000000 nifpga_fast_fifo_recv-0.99.4/Cargo.lock
+-rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.4/PKG-INFO
```

### Comparing `nifpga_fast_fifo_recv-0.99.3/LICENSE` & `nifpga_fast_fifo_recv-0.99.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.3/README.md` & `nifpga_fast_fifo_recv-0.99.4/README.md`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.3/pyproject.toml` & `nifpga_fast_fifo_recv-0.99.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.3/src/lib.rs` & `nifpga_fast_fifo_recv-0.99.4/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-extern crate nifpga;
+extern crate nifpga_dll;
 
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 use std::thread;
 use std::sync::{Arc, Mutex};
 use crossbeam;
-use nifpga::Session;
+use nifpga_dll::Session;
 
 
 #[derive(Clone)]
 #[pyclass]
 struct Configuration {
     bit_file: String,
     signature: String,
```

### Comparing `nifpga_fast_fifo_recv-0.99.3/Cargo.lock` & `nifpga_fast_fifo_recv-0.99.4/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -141,55 +141,58 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "nifpga"
-version = "0.1.5"
-source = "git+https://github.com/mattia-donato/nifpga-win-rs#bf61ce6523a4f5fa29580788675b7016a4d9f99f"
+name = "nifpga-dll"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f1010f952527f3e53713206498ac5198379304f7e5d919f6821653181a551a7"
 dependencies = [
  "fehler",
  "libc",
- "nifpga-sys",
- "nifpga-type-macro",
-]
-
-[[package]]
-name = "nifpga-fast-fifo-recv"
-version = "0.99.3"
-dependencies = [
- "cc",
- "crossbeam",
- "nifpga",
- "nifpga-sys",
- "nifpga-type-macro",
- "pyo3",
+ "nifpga-dll-sys",
+ "nifpga-dll-type-macro",
 ]
 
 [[package]]
-name = "nifpga-sys"
-version = "0.1.5"
-source = "git+https://github.com/mattia-donato/nifpga-win-rs#bf61ce6523a4f5fa29580788675b7016a4d9f99f"
+name = "nifpga-dll-sys"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c5a961585b636ff7f414d400468a7b5e44a124b8807cc73aa9e57d7ed2999b37"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "nifpga-type-macro"
-version = "0.1.5"
-source = "git+https://github.com/mattia-donato/nifpga-win-rs#bf61ce6523a4f5fa29580788675b7016a4d9f99f"
+name = "nifpga-dll-type-macro"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec34dec0ea63fa53bd0f2a36ec344ad97cfe694e889b11e2a2c7faa33446164b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
+name = "nifpga-fast-fifo-recv"
+version = "0.99.4"
+dependencies = [
+ "cc",
+ "crossbeam",
+ "nifpga-dll",
+ "nifpga-dll-sys",
+ "nifpga-dll-type-macro",
+ "pyo3",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
```

### Comparing `nifpga_fast_fifo_recv-0.99.3/PKG-INFO` & `nifpga_fast_fifo_recv-0.99.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifpga-fast-fifo-recv
-Version: 0.99.3
+Version: 0.99.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A Python module for fast reading of data from NI FPGA FIFOs with a separate thread.
 Author: Mattia Donato
 License: MIT
```

