# Comparing `tmp/stringcalc-0.1.0.dev8.tar.gz` & `tmp/stringcalc-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringcalc-0.1.0.dev8.tar", last modified: Wed Jun 14 03:07:40 2023, max compression
+gzip compressed data, was "stringcalc-0.1.0.dev9.tar", last modified: Fri Jun 23 17:58:47 2023, max compression
```

## Comparing `stringcalc-0.1.0.dev8.tar` & `stringcalc-0.1.0.dev9.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0     1533 2023-06-14 03:03:08.620029 stringcalc-0.1.0.dev8/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1974 2022-04-25 16:28:20.965299 stringcalc-0.1.0.dev8/.gitignore
--rw-r--r--   0        0        0      786 2023-05-31 22:35:00.127306 stringcalc-0.1.0.dev8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1090 2022-04-25 16:28:20.965799 stringcalc-0.1.0.dev8/LICENSE
--rw-r--r--   0        0        0      608 2023-05-31 22:01:53.642624 stringcalc-0.1.0.dev8/README.md
--rw-r--r--   0        0        0     3524 2023-03-27 18:03:35.117846 stringcalc-0.1.0.dev8/docs/prior-art.md
--rw-r--r--   0        0        0     1446 2023-06-14 03:03:08.623529 stringcalc-0.1.0.dev8/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-14 03:06:55.308398 stringcalc-0.1.0.dev8/stringcalc/__init__.py
--rw-r--r--   0        0        0    12011 2023-03-28 16:06:30.394364 stringcalc-0.1.0.dev8/stringcalc/cli.py
--rw-r--r--   0        0        0       30 2023-06-14 03:03:08.624030 stringcalc-0.1.0.dev8/stringcalc/data/__init__.py
--rw-r--r--   0        0        0     1762 2023-06-14 03:03:08.624529 stringcalc-0.1.0.dev8/stringcalc/data/aquila-nng.csv
--rw-r--r--   0        0        0   124808 2023-03-24 20:14:28.941212 stringcalc-0.1.0.dev8/stringcalc/data/daddario-tension.csv
--rw-r--r--   0        0        0      288 2023-06-14 03:03:08.625029 stringcalc-0.1.0.dev8/stringcalc/data/worth.csv
--rw-r--r--   0        0        0     3576 2023-06-14 03:03:08.626029 stringcalc-0.1.0.dev8/stringcalc/frets.py
--rw-r--r--   0        0        0    11202 2023-06-14 03:03:08.627030 stringcalc-0.1.0.dev8/stringcalc/tension.py
--rw-r--r--   0        0        0     2260 2023-06-14 03:03:08.627529 stringcalc-0.1.0.dev8/tests/test_frets.py
--rw-r--r--   0        0        0     3124 2023-06-14 03:03:08.628529 stringcalc-0.1.0.dev8/tests/test_string.py
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 stringcalc-0.1.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     2462 2023-06-20 20:03:18.732557 stringcalc-0.1.0.dev9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1974 2022-04-25 16:28:20.965299 stringcalc-0.1.0.dev9/.gitignore
+-rw-r--r--   0        0        0      786 2023-05-31 22:35:00.127306 stringcalc-0.1.0.dev9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1090 2022-04-25 16:28:20.965799 stringcalc-0.1.0.dev9/LICENSE
+-rw-r--r--   0        0        0      608 2023-05-31 22:01:53.642624 stringcalc-0.1.0.dev9/README.md
+-rw-r--r--   0        0        0     3524 2023-03-27 18:03:35.117846 stringcalc-0.1.0.dev9/docs/prior-art.md
+-rw-r--r--   0        0        0      287 2023-06-20 20:03:18.733056 stringcalc-0.1.0.dev9/panel/README.md
+-rw-r--r--   0        0        0     6423 2023-06-20 20:03:18.734056 stringcalc-0.1.0.dev9/panel/app.py
+-rw-r--r--   0        0        0      311 2023-06-20 20:03:18.734056 stringcalc-0.1.0.dev9/panel/environment.yml
+-rw-r--r--   0        0        0     1462 2023-06-20 20:03:18.735056 stringcalc-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-23 17:58:00.763579 stringcalc-0.1.0.dev9/stringcalc/__init__.py
+-rw-r--r--   0        0        0    12011 2023-03-28 16:06:30.394364 stringcalc-0.1.0.dev9/stringcalc/cli.py
+-rw-r--r--   0        0        0       30 2023-06-14 03:03:08.624030 stringcalc-0.1.0.dev9/stringcalc/data/__init__.py
+-rw-r--r--   0        0        0     1762 2023-06-14 03:03:08.624529 stringcalc-0.1.0.dev9/stringcalc/data/aquila-nng.csv
+-rw-r--r--   0        0        0   124808 2023-03-24 20:14:28.941212 stringcalc-0.1.0.dev9/stringcalc/data/daddario-tension.csv
+-rw-r--r--   0        0        0      288 2023-06-14 03:03:08.625029 stringcalc-0.1.0.dev9/stringcalc/data/worth.csv
+-rw-r--r--   0        0        0     3576 2023-06-14 03:03:08.626029 stringcalc-0.1.0.dev9/stringcalc/frets.py
+-rw-r--r--   0        0        0        0 2023-06-20 20:03:18.735056 stringcalc-0.1.0.dev9/stringcalc/py.typed
+-rw-r--r--   0        0        0    11203 2023-06-20 21:12:50.016956 stringcalc-0.1.0.dev9/stringcalc/tension.py
+-rw-r--r--   0        0        0     2260 2023-06-14 03:03:08.627529 stringcalc-0.1.0.dev9/tests/test_frets.py
+-rw-r--r--   0        0        0     3380 2023-06-20 21:13:06.743558 stringcalc-0.1.0.dev9/tests/test_string.py
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 stringcalc-0.1.0.dev9/PKG-INFO
```

### Comparing `stringcalc-0.1.0.dev8/.github/workflows/ci.yml` & `stringcalc-0.1.0.dev9/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -55,7 +55,43 @@
           cd ../stringcalc/data
           rc=0
           for f in *.csv; do
             echo $f
             cmp $f $GITHUB_WORKSPACE/stringcalc/data/$f || rc=$?
           done
           exit $rc
+
+  panel:
+    runs-on: ubuntu-latest
+    defaults:
+      run:
+        shell: bash -l {0}
+    strategy:
+      matrix:
+        stringcalc: ["local", "pypi"]
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Install dependencies (micromamba)
+        uses: mamba-org/setup-micromamba@v1
+        with:
+          environment-file: panel/environment.yml
+          cache-environment: true
+          cache-downloads: true
+
+      - name: Install stringcalc (${{ matrix.stringcalc }})
+        run: |
+          if [ "${{ matrix.stringcalc }}" == "local" ]; then
+            pip install . --no-deps
+          elif [ "${{ matrix.stringcalc }}" == "pypi" ]; then
+            pip install stringcalc
+          else
+            exit 1
+          fi
+
+      - name: Run the app script
+        run: python panel/app.py
+
+      - name: Run mypy
+        run: |
+          mypy --non-interactive panel/app.py
```

### Comparing `stringcalc-0.1.0.dev8/.gitignore` & `stringcalc-0.1.0.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/.pre-commit-config.yaml` & `stringcalc-0.1.0.dev9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/LICENSE` & `stringcalc-0.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/README.md` & `stringcalc-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/docs/prior-art.md` & `stringcalc-0.1.0.dev9/docs/prior-art.md`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/pyproject.toml` & `stringcalc-0.1.0.dev9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -62,10 +62,11 @@
 profile = "black"
 line_length = 100
 
 [tool.mypy]
 exclude = [
     "^venv/",
     "^data/",
+    "^panel/",
 ]
 install_types = true
 ignore_missing_imports = true
```

### Comparing `stringcalc-0.1.0.dev8/stringcalc/cli.py` & `stringcalc-0.1.0.dev9/stringcalc/cli.py`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/stringcalc/data/aquila-nng.csv` & `stringcalc-0.1.0.dev9/stringcalc/data/aquila-nng.csv`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/stringcalc/data/daddario-tension.csv` & `stringcalc-0.1.0.dev9/stringcalc/data/daddario-tension.csv`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/stringcalc/frets.py` & `stringcalc-0.1.0.dev9/stringcalc/frets.py`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/stringcalc/tension.py` & `stringcalc-0.1.0.dev9/stringcalc/tension.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         raise ValueError(
             f"string type IDs {sorted(types)} not found in dataset. "
             f"Use one of {sorted(data_all.group_id.cat.categories)}."
         )
 
     UW = data.uw
     F = Pitch.from_name(pitch).etf
-    T_all = UW * (2 * L * F) ** 2 / 386.0
+    T_all = UW * (2 * L * F) ** 2 / 386.09
 
     # Find closest ones
     data_sort = data.iloc[(T_all - T).abs().argsort().iloc[:n]].copy()
     data_sort["T"] = T_all[data_sort.index]
     data_sort["dT"] = data_sort["T"] - T
 
     b = 1.7  # TODO: allow to set this?
```

### Comparing `stringcalc-0.1.0.dev8/tests/test_frets.py` & `stringcalc-0.1.0.dev9/tests/test_frets.py`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev8/tests/test_string.py` & `stringcalc-0.1.0.dev9/tests/test_string.py`

 * *Files 15% similar despite different names*

```diff
@@ -120,7 +120,16 @@
 
 
 def test_load_data_categories():
     df = load_data()
 
     for name in ["category", "group", "id_pref", "id_suff", "group_id"]:
         assert df[name].dtype == "category"
+
+
+def test_string_suggest_t_consistency():
+    s = String.from_spec('25.5" PB .042')
+    P = "A2"
+    T = tension(s, pitch=P)
+    df = suggest_gauge(T, s.L, P, types={"PB"}, n=1)
+    assert df["T"].tolist() == [T]
+    assert df.dT.tolist() == [0]
```

### Comparing `stringcalc-0.1.0.dev8/PKG-INFO` & `stringcalc-0.1.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringcalc
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: Calculations for instrument strings
 Author-email: zmoon <zmoon92@gmail.com>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >=1.21
 Requires-Dist: pandas
```

