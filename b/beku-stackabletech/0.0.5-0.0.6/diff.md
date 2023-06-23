# Comparing `tmp/beku-stackabletech-0.0.5.tar.gz` & `tmp/beku_stackabletech-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beku-stackabletech-0.0.5.tar", last modified: Mon Jan 23 10:15:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

