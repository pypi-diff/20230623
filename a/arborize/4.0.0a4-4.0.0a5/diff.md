# Comparing `tmp/arborize-4.0.0a4.tar.gz` & `tmp/arborize-4.0.0a5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arborize-4.0.0a4.tar", last modified: Tue Jan 10 11:27:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

