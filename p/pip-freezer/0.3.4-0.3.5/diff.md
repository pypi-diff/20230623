# Comparing `tmp/pip-freezer-0.3.4.tar.gz` & `tmp/pip_freezer-0.3.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-freezer-0.3.4.tar", last modified: Tue Sep 14 14:03:44 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

