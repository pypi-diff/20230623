# Comparing `tmp/pyscal3-3.0.1.tar.gz` & `tmp/pyscal3-3.1.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal3-3.0.1.tar", last modified: Mon Jun 19 20:59:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

