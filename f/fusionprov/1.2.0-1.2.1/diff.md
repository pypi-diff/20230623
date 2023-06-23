# Comparing `tmp/fusionprov-1.2.0.tar.gz` & `tmp/fusionprov-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fusionprov-1.2.0.tar", last modified: Wed Oct 20 11:59:47 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

