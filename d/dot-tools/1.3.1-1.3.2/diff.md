# Comparing `tmp/dot_tools-1.3.1.tar.gz` & `tmp/dot_tools-1.3.2.tar.gz`

## Comparing `dot_tools-1.3.1.tar` & `dot_tools-1.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dot_tools-1.3.1/.coveragerc
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dot_tools-1.3.1/.editorconfig
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 dot_tools-1.3.1/.envrc
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dot_tools-1.3.1/MANIFEST.in
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dot_tools-1.3.1/README.md
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dot_tools-1.3.1/requirements.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tox.ini
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/__init__.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/resources/traefik.compose.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/scripts/__init__.py
--rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/scripts/add_dot_files.py
--rwxr-xr-x   0        0        0     2559 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/scripts/cpuniq.py
--rwxr-xr-x   0        0        0     5462 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/scripts/handle_envrc.py
--rwxr-xr-x   0        0        0     3557 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/scripts/release.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/scripts/traefik_run.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/templates/editorconfig.tmpl
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/templates/projectile.tmpl
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/templates/pyproject.tmpl
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dot_tools-1.3.1/dot_tools/templates/yamllint.tmpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.3efbc6c9873649f8aabc0f1a918d1593
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.5a53a0607caa4db19a421e2e803553f2
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.6edd2ad9ff01473e9d87d2b59ab375c8
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.70561b4a8d1c44548edeef981e812bf9
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.b9c209aecb5044f2ae36b3b53219f60b
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.d09d7ed0f38c4741887a0d87266a22bc
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb.de50b90f1d4649ec91bad8c9644cbdac
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.1/tst/bb1
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 dot_tools-1.3.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dot_tools-1.3.1/LICENSE
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 dot_tools-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 dot_tools-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dot_tools-1.3.2/.coveragerc
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dot_tools-1.3.2/.editorconfig
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 dot_tools-1.3.2/.envrc
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dot_tools-1.3.2/MANIFEST.in
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dot_tools-1.3.2/README.md
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dot_tools-1.3.2/requirements.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tox.ini
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/__init__.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/resources/traefik.compose.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/scripts/__init__.py
+-rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/scripts/add_dot_files.py
+-rwxr-xr-x   0        0        0     2707 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/scripts/cpuniq.py
+-rwxr-xr-x   0        0        0     5462 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/scripts/handle_envrc.py
+-rwxr-xr-x   0        0        0     3557 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/scripts/release.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/scripts/traefik_run.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/templates/editorconfig.tmpl
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/templates/projectile.tmpl
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/templates/pyproject.tmpl
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dot_tools-1.3.2/dot_tools/templates/yamllint.tmpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.3efbc6c9873649f8aabc0f1a918d1593
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.5a53a0607caa4db19a421e2e803553f2
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.6edd2ad9ff01473e9d87d2b59ab375c8
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.70561b4a8d1c44548edeef981e812bf9
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.b9c209aecb5044f2ae36b3b53219f60b
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.d09d7ed0f38c4741887a0d87266a22bc
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb.de50b90f1d4649ec91bad8c9644cbdac
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dot_tools-1.3.2/tst/bb1
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 dot_tools-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dot_tools-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 dot_tools-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 dot_tools-1.3.2/PKG-INFO
```

### Comparing `dot_tools-1.3.1/dot_tools/resources/traefik.compose.yaml` & `dot_tools-1.3.2/dot_tools/resources/traefik.compose.yaml`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/dot_tools/scripts/add_dot_files.py` & `dot_tools-1.3.2/dot_tools/scripts/add_dot_files.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/dot_tools/scripts/cpuniq.py` & `dot_tools-1.3.2/dot_tools/scripts/cpuniq.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 def identical_files(src: Path, dst: Path):
     """
     1. by size
     2. by hash
     """
     try:
+        if not dst.exists():
+            return False
         if src.stat().st_size != dst.stat().st_size:
             return False
         sha_src = run(['sha1sum', src], capture_output=True).stdout.split()[0]
         sha_dst = run(['sha1sum', dst], capture_output=True).stdout.split()[0]
         if sha_src != sha_dst:
             return False
         return True
@@ -87,15 +89,19 @@
 def main():
     args = parse_args()
     if args.verbose:
         log.setLevel(logging.DEBUG)
     else:
         log.setLevel(logging.WARN)
 
+    dst = Path(args.dst[0])
+    if not dst.exists():
+        log.error(f'Destination does not exist: {dst}')
+        exit(1)
+
     for fname in args.files:
         src = Path(fname)
-        dst = Path(args.dst[0])
         copy(src, dst, args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dot_tools-1.3.1/dot_tools/scripts/handle_envrc.py` & `dot_tools-1.3.2/dot_tools/scripts/handle_envrc.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/dot_tools/scripts/release.py` & `dot_tools-1.3.2/dot_tools/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/dot_tools/scripts/traefik_run.py` & `dot_tools-1.3.2/dot_tools/scripts/traefik_run.py`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/dot_tools/templates/pyproject.tmpl` & `dot_tools-1.3.2/dot_tools/templates/pyproject.tmpl`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/.gitignore` & `dot_tools-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/LICENSE` & `dot_tools-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dot_tools-1.3.1/pyproject.toml` & `dot_tools-1.3.2/pyproject.toml`

 * *Files identical despite different names*

