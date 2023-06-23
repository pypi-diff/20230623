# Comparing `tmp/astyle-3.3b3.tar.gz` & `tmp/astyle-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astyle-3.3b3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "astyle-3.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `astyle-3.3b3.tar` & `astyle-3.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 astyle-3.3b3/.github/dependabot.yml
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 astyle-3.3b3/.github/workflows/main.yml
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 astyle-3.3b3/.github/workflows/version.yml
--rw-r--r--   0        0        0     2346 2022-11-09 12:37:21.000000 astyle-3.3b3/.gitignore
--rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 astyle-3.3b3/.gitlint
--rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 astyle-3.3b3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 astyle-3.3b3/.pre-commit-hooks.yaml
--rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 astyle-3.3b3/.yamllint.yaml
--rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 astyle-3.3b3/CMakeLists.txt
--rw-r--r--   0        0        0     4968 2022-11-09 12:37:21.000000 astyle-3.3b3/README.md
--rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 astyle-3.3b3/pyproject.toml
--rwxr-xr-x   0        0        0      784 2022-11-09 12:37:21.000000 astyle-3.3b3/scripts/git-commit.sh
--rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 astyle-3.3b3/src/astyle/__init__.py
--rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 astyle-3.3b3/src/astyle/__main__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 astyle-3.3b3/src/astyle/py.typed
--rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 astyle-3.3b3/tests/astyle_test.py
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 astyle-3.3b3/tests/expected.c
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 astyle-3.3b3/tests/input.c
--rw-r--r--   0        0        0     6456 2022-11-09 12:37:21.000000 astyle-3.3b3/PKG-INFO
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 astyle-3.4/.cmake-format.yaml
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 astyle-3.4/.cmakelintrc
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 astyle-3.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 astyle-3.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 astyle-3.4/.github/workflows/version.yml
+-rw-r--r--   0        0        0     2346 2022-11-09 12:37:21.000000 astyle-3.4/.gitignore
+-rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 astyle-3.4/.gitlint
+-rw-r--r--   0        0        0     3293 2022-11-09 12:37:21.000000 astyle-3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 astyle-3.4/.pre-commit-hooks.yaml
+-rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 astyle-3.4/.yamllint.yaml
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 astyle-3.4/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 astyle-3.4/LICENSE
+-rw-r--r--   0        0        0     5464 2022-11-09 12:37:21.000000 astyle-3.4/README.md
+-rw-r--r--   0        0        0     2135 2022-11-09 12:37:21.000000 astyle-3.4/pyproject.toml
+-rwxr-xr-x   0        0        0      774 2022-11-09 12:37:21.000000 astyle-3.4/scripts/git-commit.sh
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 astyle-3.4/src/astyle/__init__.py
+-rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 astyle-3.4/src/astyle/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 astyle-3.4/src/astyle/py.typed
+-rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 astyle-3.4/tests/astyle_test.py
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 astyle-3.4/tests/expected.c
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 astyle-3.4/tests/input.c
+-rw-r--r--   0        0        0     6950 2022-11-09 12:37:21.000000 astyle-3.4/PKG-INFO
```

### Comparing `astyle-3.3b3/.github/workflows/main.yml` & `astyle-3.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `astyle-3.3b3/.gitignore` & `astyle-3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `astyle-3.3b3/.pre-commit-config.yaml` & `astyle-3.4/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -43,16 +43,20 @@
   - repo: https://github.com/jumanjihouse/pre-commit-hooks
     rev: 3.0.0
     hooks:
       - id: check-mailmap
       - id: shellcheck
         exclude_types:
           - zsh
+  - repo: https://github.com/rhysd/actionlint
+    rev: v1.6.24
+    hooks:
+      - id: actionlint
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.31.0
+    rev: v1.32.0
     hooks:
       - id: yamllint
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies:
@@ -85,28 +89,42 @@
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies:
           - tomli
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.308
+    rev: v1.1.309
     hooks:
       - id: pyright
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - -cpyproject.toml
         additional_dependencies:
           - tomli
+  - repo: https://github.com/cmake-lint/cmake-lint
+    rev: 1.4.2
+    hooks:
+      - id: cmakelint
+  - repo: https://github.com/cheshirekow/cmake-format-precommit
+    rev: v0.6.13
+    hooks:
+      - id: cmake-format
+        additional_dependencies:
+          - pyyaml
+      - id: cmake-lint
+        additional_dependencies:
+          - pyyaml
   - repo: https://github.com/Freed-Wu/astyle-wheel
-    rev: 3.3-beta3
+    rev: "3.3"
     hooks:
       - id: astyle
         exclude: ^tests/input\.c$
 
 ci:
   skip:
+    - actionlint
     - shellcheck
     - pyright
```

### Comparing `astyle-3.3b3/README.md` & `astyle-3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -65,29 +65,38 @@
 
 ### pre-commit
 
 `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
-  - repo: https://github.com/Freed-Wu/astyle-wheel
-    rev: 3.3-beta3
+  - repo: https://github.com/Freed-Wu/mirrors-astyle
+    rev: 3.4
     hooks:
       - id: astyle
 ```
 
 ```shell
 pre-commit install
 git commit
 ```
 
+Please use <https://github.com/Freed-Wu/mirrors-astyle>, it uses binary wheel
+and will be faster than this repository which uses source code.
+
 ## Similar Projects
 
 ### pre-commit hooks
 
 - [mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format)
+- [astyle_precommit_hook](https://github.com/mellowcandle/astyle_precommit_hook):
+  it uses git hook, not pre-commit, which make it cannot use many hooks at the
+  same time.
+- [pyastyle](https://github.com/timonwong/pyastyle): stop maintaining.
+- [astyle_py](https://github.com/igrr/astyle_py): it uses wasm, not native
+  binary programs like this project.
 
 ### Python distributions
 
 - [clang-format-wheel](https://github.com/ssciwr/clang-format-wheel)
 - [cmake-python-distributions](https://github.com/scikit-build/cmake-python-distributions)
 - [ninja-python-distributions](https://github.com/scikit-build/ninja-python-distributions)
```

### Comparing `astyle-3.3b3/pyproject.toml` & `astyle-3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core"]
 build-backend = "scikit_build_core.build"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "astyle"
-version = "3.3-beta3"
+version = "3.4"
 description = "Artistic Style is a source code indenter, formatter, and beautifier for the C, C++, C++/CLI, Objective‑C, C# and Java programming languages"
 readme = "README.md"
 requires-python = ">= 3.7"
 keywords = ["astyle"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `astyle-3.3b3/scripts/git-commit.sh` & `astyle-3.4/scripts/git-commit.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env bash
 cd "$(dirname "$(readlink -f "$0")")/.." || exit 1
 
 version="$(curl 'https://gitlab.com/api/v4/projects/41218592/repository/tags?per_page=1' | jq -r '.[].name')"
 perl -pi -e's/(?<=^version = ")[^"]+(?="$)/'"$version/" pyproject.toml
 [ -n "$(git diff)" ] || exit
 perl -pi -e's/(?<=^    rev: )\S+/'"$version/" README.md
-perl -pi -e's/(?<=^set\(VERSION )\S+(?=\)$)/'"$version/" CMakeLists.txt
+perl -pi -e's/(?<=^set\(VERSION )\S+)/'"$version/" CMakeLists.txt
 
 git add pyproject.toml README.md CMakeLists.txt
 git config --global user.name 'Github Actions'
 git config --global user.email '41898282+github-actions[bot]@users.noreply.github.com'
 git commit -m ":bookmark: Dump version to $version"
 git tag "$version"
-git remote set-url origin "https://x-access-token:$GITHUB_TOKEN@github.com/$GITHUB_REPOSITORY"
+git remote set-url origin "https://x-access-token:$GH_TOKEN@github.com/$GITHUB_REPOSITORY"
 git push
 git push --tags
```

### Comparing `astyle-3.3b3/tests/astyle_test.py` & `astyle-3.4/tests/astyle_test.py`

 * *Files identical despite different names*

### Comparing `astyle-3.3b3/PKG-INFO` & `astyle-3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astyle
-Version: 3.3b3
+Version: 3.4
 Summary: Artistic Style is a source code indenter, formatter, and beautifier for the C, C++, C++/CLI, Objective‑C, C# and Java programming languages
 Keywords: astyle
 Author-Email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -96,29 +96,38 @@
 
 ### pre-commit
 
 `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
-  - repo: https://github.com/Freed-Wu/astyle-wheel
-    rev: 3.3-beta3
+  - repo: https://github.com/Freed-Wu/mirrors-astyle
+    rev: 3.4
     hooks:
       - id: astyle
 ```
 
 ```shell
 pre-commit install
 git commit
 ```
 
+Please use <https://github.com/Freed-Wu/mirrors-astyle>, it uses binary wheel
+and will be faster than this repository which uses source code.
+
 ## Similar Projects
 
 ### pre-commit hooks
 
 - [mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format)
+- [astyle_precommit_hook](https://github.com/mellowcandle/astyle_precommit_hook):
+  it uses git hook, not pre-commit, which make it cannot use many hooks at the
+  same time.
+- [pyastyle](https://github.com/timonwong/pyastyle): stop maintaining.
+- [astyle_py](https://github.com/igrr/astyle_py): it uses wasm, not native
+  binary programs like this project.
 
 ### Python distributions
 
 - [clang-format-wheel](https://github.com/ssciwr/clang-format-wheel)
 - [cmake-python-distributions](https://github.com/scikit-build/cmake-python-distributions)
 - [ninja-python-distributions](https://github.com/scikit-build/ninja-python-distributions)
```

