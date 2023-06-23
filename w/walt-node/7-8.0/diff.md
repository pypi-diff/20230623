# Comparing `tmp/walt-node-7.tar.gz` & `tmp/walt_node-8.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walt-node-7.tar", last modified: Mon Feb  1 15:17:02 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

