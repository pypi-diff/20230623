# Comparing `tmp/pyparaspace-0.1.3.tar.gz` & `tmp/pyparaspace-0.1.4.tar.gz`

## Comparing `pyparaspace-0.1.3.tar` & `pyparaspace-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 pyparaspace-0.1.3/local_dependencies/paraspace/Cargo.toml
--rw-r--r--   0        0        0     1106 2023-06-17 17:54:52.000000 pyparaspace-0.1.3/local_dependencies/paraspace/LICENSE
--rw-r--r--   0        0        0      165 2023-06-17 17:54:52.000000 pyparaspace-0.1.3/local_dependencies/paraspace/README.md
--rw-r--r--   0        0        0     1097 2023-06-17 17:54:52.000000 pyparaspace-0.1.3/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt
--rw-r--r--   0        0        0     1315 2023-06-17 17:54:52.000000 pyparaspace-0.1.3/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt
--rw-r--r--   0        0        0     2640 2023-06-17 17:54:52.000000 pyparaspace-0.1.3/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt
--rw-r--r--   0        0        0        0 2023-06-17 17:54:52.000000 pyparaspace-0.1.3/local_dependencies/paraspace/examples/.emptydir
--rw-r--r--   0        0        0      130 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/scripts/mkbenchmarks.sh
--rw-r--r--   0        0        0     3795 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/scripts/plot_timeline.py
--rw-r--r--   0        0        0     1626 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/cores.rs
--rw-r--r--   0        0        0     2128 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/carbonaraproblem.py
--rw-r--r--   0        0        0     2079 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/ceramicproblem.py
--rw-r--r--   0        0        0     2422 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/goacproblem.py
--rw-r--r--   0        0        0     4776 2023-06-17 17:54:53.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/timelinedsl.py
--rw-r--r--   0        0        0      886 2023-06-21 14:17:33.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/lib.rs
--rw-r--r--   0        0        0     3853 2023-06-21 14:17:33.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/main.rs
--rw-r--r--   0        0        0     2336 2023-06-21 14:17:33.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/problem.rs
--rw-r--r--   0        0        0    67590 2023-06-21 14:17:33.000000 pyparaspace-0.1.3/local_dependencies/paraspace/src/transitionsolver.rs
--rw-r--r--   0        0        0     3565 2023-06-21 14:17:33.000000 pyparaspace-0.1.3/local_dependencies/paraspace/tests/transitions_1.rs
--rw-r--r--   0        0        0     2385 2023-06-21 14:17:33.000000 pyparaspace-0.1.3/local_dependencies/paraspace/tests/transitions_2.rs
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 pyparaspace-0.1.3/Cargo.toml
--rw-r--r--   0        0        0      756 2023-06-17 17:54:48.000000 pyparaspace-0.1.3/.gitignore
--rw-r--r--   0        0        0      102 2023-06-17 17:54:48.000000 pyparaspace-0.1.3/.gitmodules
--rw-r--r--   0        0        0      869 2023-06-21 15:00:11.000000 pyparaspace-0.1.3/Dockerfile
--rw-r--r--   0        0        0     1723 2023-06-17 17:54:48.000000 pyparaspace-0.1.3/README.md
--rw-r--r--   0        0        0      390 2023-06-17 17:54:48.000000 pyparaspace-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    15142 2023-06-21 15:00:11.000000 pyparaspace-0.1.3/src/lib.rs
--rw-r--r--   0        0        0     1924 2023-06-21 14:16:28.000000 pyparaspace-0.1.3/testPyParaspace.py
--rw-r--r--   0        0        0    20342 2023-06-21 15:02:37.000000 pyparaspace-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 pyparaspace-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 pyparaspace-0.1.4/local_dependencies/paraspace/Cargo.toml
+-rw-r--r--   0        0        0     1106 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/README.md
+-rw-r--r--   0        0        0     1097 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt
+-rw-r--r--   0        0        0     1315 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt
+-rw-r--r--   0        0        0     2640 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt
+-rw-r--r--   0        0        0        0 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/examples/.emptydir
+-rw-r--r--   0        0        0      130 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/scripts/mkbenchmarks.sh
+-rw-r--r--   0        0        0     3795 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/scripts/plot_timeline.py
+-rw-r--r--   0        0        0     1626 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/cores.rs
+-rw-r--r--   0        0        0     2128 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/carbonaraproblem.py
+-rw-r--r--   0        0        0     2079 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/ceramicproblem.py
+-rw-r--r--   0        0        0     2422 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/goacproblem.py
+-rw-r--r--   0        0        0     4776 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/timelinedsl.py
+-rw-r--r--   0        0        0      886 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/lib.rs
+-rw-r--r--   0        0        0     3853 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/main.rs
+-rw-r--r--   0        0        0     2373 2023-06-23 12:37:36.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/problem.rs
+-rw-r--r--   0        0        0    69611 2023-06-23 12:37:36.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/transitionsolver.rs
+-rw-r--r--   0        0        0     3565 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_1.rs
+-rw-r--r--   0        0        0     2385 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_2.rs
+-rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 pyparaspace-0.1.4/Cargo.toml
+-rw-r--r--   0        0        0      756 2023-06-17 17:54:48.000000 pyparaspace-0.1.4/.gitignore
+-rw-r--r--   0        0        0      102 2023-06-17 17:54:48.000000 pyparaspace-0.1.4/.gitmodules
+-rw-r--r--   0        0        0      869 2023-06-21 15:00:11.000000 pyparaspace-0.1.4/Dockerfile
+-rw-r--r--   0        0        0     1923 2023-06-23 12:37:18.000000 pyparaspace-0.1.4/README.md
+-rw-r--r--   0        0        0      390 2023-06-17 17:54:48.000000 pyparaspace-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    15373 2023-06-23 12:37:18.000000 pyparaspace-0.1.4/src/lib.rs
+-rw-r--r--   0        0        0     1932 2023-06-23 12:37:18.000000 pyparaspace-0.1.4/testPyParaspace.py
+-rw-r--r--   0        0        0    20342 2023-06-23 12:37:22.000000 pyparaspace-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 pyparaspace-0.1.4/PKG-INFO
```

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/LICENSE` & `pyparaspace-0.1.4/local_dependencies/paraspace/LICENSE`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt` & `pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt` & `pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt` & `pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/scripts/plot_timeline.py` & `pyparaspace-0.1.4/local_dependencies/paraspace/scripts/plot_timeline.py`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/cores.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/cores.rs`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/carbonaraproblem.py` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/carbonaraproblem.py`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/ceramicproblem.py` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/ceramicproblem.py`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/goacproblem.py` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/goacproblem.py`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/frontend/timelinedsl.py` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/timelinedsl.py`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/lib.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/main.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/problem.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/problem.rs`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
 #[derive(Serialize, Deserialize, Debug)]
 pub enum TemporalRelationship {
     MetBy,
     MetByTransitionFrom,
     Meets,
     Starts,
+    StartPrecond,
+    StartEffect,
     Cover,
     Equal,
     StartsAfter,
 }
 
 //
 // SOLUTION
```

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/src/transitionsolver.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/src/transitionsolver.rs`

 * *Files 2% similar despite different names*

```diff
@@ -790,14 +790,48 @@
                                     &states[tokens[conds[cond_idx].token_idx].state].start_time,
                                 ),
                                 Real::le(
                                     &states[tokens[conds[cond_idx].token_idx].state].end_time,
                                     &states[tokens[token_idx].state].end_time,
                                 ),
                             ],
+                            TemporalRelationship::StartPrecond => vec![
+                                Real::le(
+                                    &Real::add(
+                                        &ctx,
+                                        &[
+                                            &states[tokens[conds[cond_idx].token_idx].state]
+                                                .start_time,
+                                            &Real::from_real(&ctx, 1_i32, 1), // TODO configurable epsilon
+                                        ],
+                                    ),
+                                    &states[tokens[token_idx].state].start_time,
+                                ),
+                                Real::le(
+                                    &states[tokens[token_idx].state].start_time,
+                                    &states[tokens[conds[cond_idx].token_idx].state].end_time,
+                                ),
+                            ],
+                            TemporalRelationship::StartEffect => vec![
+                                Real::le(
+                                    &states[tokens[conds[cond_idx].token_idx].state].start_time,
+                                    &states[tokens[token_idx].state].start_time,
+                                ),
+                                Real::le(
+                                    &states[tokens[token_idx].state].start_time,
+                                    &Real::add(
+                                        &ctx,
+                                        &[
+                                            &states[tokens[conds[cond_idx].token_idx].state]
+                                                .end_time,
+                                            &Real::from_real(&ctx, 1_i32, 1), // TODO configurable epsilon
+                                        ],
+                                    ),
+                                ),
+                            ],
                             TemporalRelationship::Equal => vec![
                                 Real::_eq(
                                     &states[tokens[token_idx].state].start_time,
                                     &states[tokens[conds[cond_idx].token_idx].state].start_time,
                                 ),
                                 Real::_eq(
                                     &states[tokens[conds[cond_idx].token_idx].state].end_time,
```

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/tests/transitions_1.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_1.rs`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/local_dependencies/paraspace/tests/transitions_2.rs` & `pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_2.rs`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/.gitignore` & `pyparaspace-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/Dockerfile` & `pyparaspace-0.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyparaspace-0.1.3/README.md` & `pyparaspace-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,7 +50,13 @@
 ## Manylinux
 
 `paraspace` requires an Rust version 1.60 and Clang version 3.5 (to compile the Z3 solver), 
 which makes it requires a bit of setup to correcly build the manylinux wheel. 
 There is a Dockerfile available that can be used to build a Docker image with 
 an up-to-date Rust version and version 7 of the LLVM/Clang toolchain.
 
+The builds should work using the following commands.
+```
+docker build -t mybuild .
+docker run --rm -v $(pwd):/io mybuild publish --skip-existing --compatibility manylinux2014 -i python3.10
+```
+
```

### Comparing `pyparaspace-0.1.3/src/lib.rs` & `pyparaspace-0.1.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,16 @@
 #[pyclass(name = "TemporalRelation")]
 #[derive(Clone, Debug)]
 pub enum TemporalRelationPy {
     MetBy,
     MetByTransitionFrom,
     Meets,
     Starts,
+    StartPrecond,
+    StartEffect,
     Cover,
     Equal,
     StartsAfter,
 }
 
 //
 // SOLUTION
@@ -569,13 +571,16 @@
                             TemporalRelationship::MetByTransitionFrom
                         }
                         TemporalRelationPy::Meets => TemporalRelationship::Meets,
                         TemporalRelationPy::Cover => TemporalRelationship::Cover,
                         TemporalRelationPy::Equal => TemporalRelationship::Equal,
                         TemporalRelationPy::StartsAfter => TemporalRelationship::StartsAfter,
                         TemporalRelationPy::Starts => TemporalRelationship::Starts,
+                        TemporalRelationPy::StartPrecond => TemporalRelationship::StartPrecond,
+                        TemporalRelationPy::StartEffect => TemporalRelationship::StartEffect,
                     },
                 })
                 .collect()
         })
         .collect()
 }
+
```

### Comparing `pyparaspace-0.1.3/testPyParaspace.py` & `pyparaspace-0.1.4/testPyParaspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 def test_pyparaspace():
     problem = pyparaspace.Problem(
         timelines=[
             pyparaspace.Timeline(
                 name="obj",
                 token_types=[
-                    pyparaspace.Value(
+                    pyparaspace.TokenType(
                         value="s1", conditions=[], duration_limits=(5, 6), capacity=0
                     ),
-                    pyparaspace.Value(
+                    pyparaspace.TokenType(
                         value="s2",
                         conditions=[
                             pyparaspace.TemporalCond(
                                 temporal_relation=pyparaspace.TemporalRelation.MetBy,
                                 amount=0,
                                 timeline="obj",
                                 value="s1",
```

### Comparing `pyparaspace-0.1.3/Cargo.lock` & `pyparaspace-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyparaspace"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "indexmap",
  "paraspace",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `pyparaspace-0.1.3/PKG-INFO` & `pyparaspace-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparaspace
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 `pyparaspace`: a Python wrapper for the [ParaSpace timelines planner](https://github.com/luteberget/paraspace) -- a simple, flexible and extensible solver for timeline-based planning problems using the [Z3 Theorem Prover](https://github.com/Z3Prover/z3).
@@ -59,8 +59,14 @@
 ## Manylinux
 
 `paraspace` requires an Rust version 1.60 and Clang version 3.5 (to compile the Z3 solver), 
 which makes it requires a bit of setup to correcly build the manylinux wheel. 
 There is a Dockerfile available that can be used to build a Docker image with 
 an up-to-date Rust version and version 7 of the LLVM/Clang toolchain.
 
+The builds should work using the following commands.
+```
+docker build -t mybuild .
+docker run --rm -v $(pwd):/io mybuild publish --skip-existing --compatibility manylinux2014 -i python3.10
+```
+
```

