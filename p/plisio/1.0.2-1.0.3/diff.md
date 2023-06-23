# Comparing `tmp/plisio-1.0.2.tar.gz` & `tmp/plisio-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plisio-1.0.2.tar", last modified: Tue Apr  5 08:47:01 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

