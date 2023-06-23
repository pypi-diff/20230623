# Comparing `tmp/dot_tools-1.2.0.tar.gz` & `tmp/dot_tools-1.3.0.tar.gz`

## Comparing `dot_tools-1.2.0.tar` & `dot_tools-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,33 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dot_tools-1.2.0/.coveragerc
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dot_tools-1.2.0/.editorconfig
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dot_tools-1.2.0/MANIFEST.in
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dot_tools-1.2.0/README.md
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dot_tools-1.2.0/requirements.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dot_tools-1.2.0/tox.ini
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/__init__.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/resources/traefik.compose.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/scripts/__init__.py
--rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/scripts/add_dot_files.py
--rwxr-xr-x   0        0        0     5462 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/scripts/handle_envrc.py
--rwxr-xr-x   0        0        0     3557 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/scripts/release.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/scripts/traefik_run.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/templates/editorconfig.tmpl
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/templates/projectile.tmpl
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/templates/pyproject.tmpl
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dot_tools-1.2.0/dot_tools/templates/yamllint.tmpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 dot_tools-1.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dot_tools-1.2.0/LICENSE
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dot_tools-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 dot_tools-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dot_tools-1.3.0/.coveragerc
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dot_tools-1.3.0/.editorconfig
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 dot_tools-1.3.0/.envrc
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dot_tools-1.3.0/MANIFEST.in
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dot_tools-1.3.0/README.md
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dot_tools-1.3.0/requirements.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tox.ini
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/__init__.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/resources/traefik.compose.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/scripts/__init__.py
+-rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/scripts/add_dot_files.py
+-rwxr-xr-x   0        0        0     2559 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/scripts/cpuniq.py
+-rwxr-xr-x   0        0        0     5462 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/scripts/handle_envrc.py
+-rwxr-xr-x   0        0        0     3557 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/scripts/release.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/scripts/traefik_run.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/templates/editorconfig.tmpl
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/templates/projectile.tmpl
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/templates/pyproject.tmpl
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dot_tools-1.3.0/dot_tools/templates/yamllint.tmpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.3efbc6c9873649f8aabc0f1a918d1593
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.5a53a0607caa4db19a421e2e803553f2
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.6edd2ad9ff01473e9d87d2b59ab375c8
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.70561b4a8d1c44548edeef981e812bf9
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.b9c209aecb5044f2ae36b3b53219f60b
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.d09d7ed0f38c4741887a0d87266a22bc
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb.de50b90f1d4649ec91bad8c9644cbdac
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.0/tst/bb1
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 dot_tools-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dot_tools-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 dot_tools-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 dot_tools-1.3.0/PKG-INFO
```

### Comparing `dot_tools-1.2.0/dot_tools/resources/traefik.compose.yaml` & `dot_tools-1.3.0/dot_tools/resources/traefik.compose.yaml`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/dot_tools/scripts/add_dot_files.py` & `dot_tools-1.3.0/dot_tools/scripts/add_dot_files.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/dot_tools/scripts/handle_envrc.py` & `dot_tools-1.3.0/dot_tools/scripts/handle_envrc.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/dot_tools/scripts/release.py` & `dot_tools-1.3.0/dot_tools/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/dot_tools/scripts/traefik_run.py` & `dot_tools-1.3.0/dot_tools/scripts/traefik_run.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/dot_tools/templates/pyproject.tmpl` & `dot_tools-1.3.0/dot_tools/templates/pyproject.tmpl`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/.gitignore` & `dot_tools-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/LICENSE` & `dot_tools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dot_tools-1.2.0/pyproject.toml` & `dot_tools-1.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 github = 'https://github.com/cybergrind/dot-tools'
 
 [project.scripts]
 'release.py' = 'dot_tools.scripts.release:main'
 handle_envrc = 'dot_tools.scripts.handle_envrc:main'
 add_dot_files = 'dot_tools.scripts.add_dot_files:main'
 traefik_run = 'dot_tools.scripts.traefik_run:main'
+cpuniq = 'dot_tools.scripts.cpuniq'
 
 [requires]
 python_version = ['3.5', '3.6', '3.7']
 
 [build-system]
 requires = ['setuptools', 'wheel', 'hatchling']
 build-backend = 'hatchling.build'
```

